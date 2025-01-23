---
layout: project
type: project
image: img/coin.webp
title: "spamMusubi"
date: 2024
published: true
labels:
  - C
summary: "This is a program in C I made while taking ICS 212 that simulates a coin flip"
---

/*
 * This program will simulate flipping a coin.
 * The user will input the number of times the coin will flip.
 * The output will print the number of times the coin flipped on both heads 
 * and tails. 
 * The program will also print the percentage of times the coin flipped on 
 * heads and tails.
 *
 * @author     Maramara, Mateo
 * @assignment ICS 212 Assignment 08
 * @date       September 26, 2024
 */
#include <stdio.h>
#include "getdouble.h"

int main() {
  srand(time(NULL));
  //declare variables to store number of heads and tails
  int heads = 0;
  int tails = 0;
  int numFlips;

  //Ask for user input
  printf("Coin Flip Simulator\n");
  printf("How many times do you want to flip the coin?");
  numFlips = (int) getdouble();

  //Number of flips must cannot be less than 1
  if (numFlips>=1){
  //declare variable for loop
  int i;
  for(i=0; i<numFlips; i++) {
    //Declare variable to store a random flip on either side 
    int flip = rand() % 2; 
    if (flip==0){
      heads++;
    } else{
      tails++;
    }
  }

  //Percentage breakdown of heads and tails formula
  double percentHeads = 100.0 * heads / numFlips;
  double percentTails = 100.0 * tails / numFlips;

  //Print number of flips on heads and tails
  printf("Number of Heads: %d\n", heads);
  printf("Number of Tails: %d\n", tails);

  //Print percentage of heads and tails
  printf("Percentage of Heads: %.2f%%\n", percentHeads);
  printf("Percentage of Tails: %.2f%%\n", percentTails);

  return 0;

  } else {
    //Message for invalid input
    printf("Error: Please enter an integer greater than or equal to 1.");
    return 0;
  }
}

program: coinFlip.o getdouble.o
	gcc coinFlip.o getdouble.o -o program

coinFlip.o: coinFlip.c getdouble.h
	gcc -c coinFlip.c

getdouble.o: getdouble.c getdouble.h
	gcc -c getdouble.c



