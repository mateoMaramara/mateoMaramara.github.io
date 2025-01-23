---
layout: project
type: project
image: img/heart.jpg
title: "heartRateCalculator"
date: 2024
published: true
labels:
  - C
summary: "This is a program in C I made while taking ICS 212 that will calculate a persons target heart rate based off of their age."
---

/**
 * This program will calculate a persons target heart rate based off of their
 * age. The required user input will be the users birth year and the current 
 * year. The expected output should be the users age, maximum heart rate, and 
 * target heart rate.
 */
#include <stdio.h>
#include "getdouble.h"

//Symbolic constant for the maximum heart rate
#define MAX_HEART_RATE 220

int main() {

  //Informs the user what the program will do
  puts("This program will calculate your target heart-rate for exercising. ");

  //Declare variable
  int birthYear;
  //Get users input for birth year
  printf("Please enter the year you were born: ");
  birthYear =(int)getdouble();

  //Declare variable
  int currentYear;
  //Get users input for current year
  printf("Please enter the current year: ");
  currentYear =(int)getdouble();

  //Declare variable
  int age;
  //Apply age formula to get users age
  age = currentYear - birthYear;

  //Declare variable
  int maxHeartRate;
  //Apply maximum heart rate formula to get the users maximum heart rate
  maxHeartRate = MAX_HEART_RATE - age;

  //Declare variable
  int lowerTarget;
  int upperTarget;
  //Apply maximum heart rate formula to get users maximum heart rate
  lowerTarget =(int)(maxHeartRate * 0.50);
  upperTarget =(int)(maxHeartRate * 0.85);
  
  //Output of age, max heart rate, and target heart rate
  printf("Your age is: %i\n", age);
  printf("Your maximum heart-rate is: %i\n", maxHeartRate);
  printf("Your target heart-rate is between %i and %i beats per minute.\n", lowerTarget, upperTarget);

  return 0;
}
program: heartRateCalculator.o getdouble.o
	gcc heartRateCalculator.o getdouble.o -o program -lm

heartRateCalculator.o: heartRateCalculator.c getdouble.h
	gcc -c heartRateCalculator.c

getdouble.o: getdouble.c getdouble.h
	gcc -c getdouble.c

