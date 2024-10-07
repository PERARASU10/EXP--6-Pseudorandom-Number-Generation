# EXP--6-Pseudorandom-Number-Generation

## Exp 6 - Implementation of Pseudorandom Number Generation using Standard library

## AIM : -
To implement Pseudorandom Number Generation using Standard Library.

## ALGORITHM : -
Step 1: Get the number of random numbers to generate from the user.

Step 2: Read the minimum and maximum values for the random number range.

Step 3: Initialize the random seed using the current time.

Step 4: Generate a random number by calculating the remainder of division with the range 
(max - min + 1) and adding the minimum value.

Step 5: Repeat the random number generation for the specified count.

Step 6: Print each generated random number.

Step 7: End the program.

## PROGRAM : -
```
#include <stdio.h>
#include <stdlib.h>
#include <time.h>
int main() 
{
printf("Pseudorandom-Number-Generation");
 int count, min, max;
 printf("Enter the number of random numbers to generate: ");
 scanf("%d", &count);
 printf("Enter the minimum value: ");
 scanf("%d", &min);
 printf("Enter the maximum value: ");
 scanf("%d", &max);
 srand(time(NULL));
 printf("Pseudorandom numbers:\n");
 
 for (int i = 0; i < count; i++) 
 {
 int random_number = (rand() % (max - min + 1)) + min;
 printf("%d\n", random_number);
 }
 return 0;
}
```
## OUTPUT : -

![image](https://github.com/user-attachments/assets/9ffa0727-2051-4ab0-a0b5-a7af2a112f0e)

## RESULT : -
The program for Pseudorandom Number Generation is executed successfully.
