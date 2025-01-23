---
layout: project
type: project
image: img/musubi.jpeg
title: "spamMusubi"
date: 2024
published: true
labels:
  - C
summary: "This is a program in C I made while taking ICS 212 that will print my favorite food in a way that practices using the modulo operator"
---

/**
 * This program will print numbers 1-100 with the exception of: 
 * Numbers divisible by 3: "Spam" will be printed instead of the number.
 * Numbers divisible by 7: "Musubi" Will be printed instead of the number.
 * Numbers divisible by both 3 and 7: "SpamMusubi" will be printed instead of
 * the number.
 */
#include <stdio.h>

int main() {

  //Printed program description using for-loop
  puts("\nSpamMusubi Algorithim using a for-loop:");
  
  //Declare variable
  int i;
  //for loop will print numbers 1-100
  for(i=1; i<=100; i++){
    //If number is divisible by both 3 and 7
    if(i%3==0 && i%7==0){
      printf("SpamMusubi\n");
      //If number is divisible only by 3
    } else if (i%3==0){
      printf("Spam\n");
      //If number is divisible only by 7
    } else if (i%7==0){
      printf("Musubi\n");
      //All cases where the number itself must be printed.
    } else {
      printf("%d\n", i); 
    }
  }
  //Printed program description using while-loop
  puts("\nSpamMusubi algorithm using a while-loop:");
  //Declare variable
  int j=1;
  while(j<=100){
    //If number is divisible by both 3 and 7                                   
    if(j%3==0 && j%7==0){
      printf("SpamMusubi\n");
      //If number is divisible only by 3                                       
    } else if (j%3==0){
      printf("Spam\n");
      //If number is divisible only by 7                                       
    } else if (j%7==0){
      printf("Musubi\n");
      //All cases where the number itself must be printed.                     
    } else {
      printf("%d\n", j);
    }
    j++;
  }
  return 0;
}

program: spamMusubi.o
	gcc spamMusubi.o -o program

spamMusubi.o: spamMusubi.c
	gcc -c spamMusubi.c 

