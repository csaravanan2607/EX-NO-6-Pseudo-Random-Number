# Pseudo Random Number
# Implementation of pseudorandom number generation using standard library
## Aim:
To write a C program to implement the pseudorandom number generation using standard library.
## ALGORITHM:
### STEP-1: Start the program and import the required libraries.
### STEP-2: Seed the random number generator using the current time(i.e) rand(time(0));
### STEP-3: Get the number of randon number to generate.
### STEP-4: Pass the value for number of iterations and print the numbers.
### STEP-5: End the program.

## PROGRAM:
```
 #include <stdio.h>
 #include <stdlib.h>
 #include <time.h>
 int main()
 {
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
 int random_number = (rand() % (max- min + 1)) + min;
 printf("%d\n", random_number);
 }
 return 0;
 }
```
# OUTPUT:
 ![Screenshot 2025-04-07 085453](https://github.com/user-attachments/assets/c47de992-4720-4fd5-b3fb-69232aacba87)

# RESULT:
Thus,the program is executed successfully.
