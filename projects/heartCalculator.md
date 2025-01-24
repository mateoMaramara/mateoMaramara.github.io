---
layout: project
type: project
image: img/heart.jpg
title: "Heart Rate Calculator"
date: 2024
published: true
labels:
  - C
summary: "This is a program in C I made while taking ICS 212 that will calculate a persons target heart rate based off of their age."
---

The “Heart Rate Calculator” is a program I made while taking ICS 212. It asks for the users “birth year” and “current year”, then determines their age. Based on their age, it calculates the “target heart rate” for workouts. It does so by first subtracting the birth year from the current year and stores it in the “age” object. To calculate the “Maximum heart rate” it subtracts the age from 220 and uses this number to calculate the “Target heart rate”. The target heart rate is calculated as 50% to 85% of the maximum heart rate. With the user input as their birth year and the current year, the output should look like the example below. 
	
The program was designed for my class to practice input handling, arithmetic operations, and formatted output. This was one of the earlier projects we did in the class that used a custom getdouble() function. Working on this project allowed me to practice making code with clear and user friendly outputs. I really enjoyed this assignment because it really is a good example of how programming can be applied to almost any subject, including fitness and health.

---

Expected Output:

Enter your birth year: 1997
Enter the current year: 2025  

Your age is: 28 years  
Your maximum heart rate is: 192 bpm  
Your target heart rate range is: 96 bpm to 163 bpm  

---

URL to repository: http://github.com/mateoMaramara/heartRateCalculator
