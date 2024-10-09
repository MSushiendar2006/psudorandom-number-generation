#   Pseudorandom-Number-Generation
# Cryptography---19CS412-classical-techqniques
Pseudo Rndom number generation with random values

# AIM:
To encrypt and decrypt the given message by using pseudo random number generation algorithm.

## DESIGN STEPS:
### Step 1:
Start the program.
### Step 2:
Implementation using C or pyton code.
### Step 3:
Get the number of random numbers to generate from the user.
### Step 4:
Read the minimum and maximum values for the random number range.
### Step 5: 
Initialize the random seed using the current time.
### Step 6:
Generate a random number by calculating the remainder of division with the range 
(max - min + 1) and adding the minimum value.
### Step 7: 
Repeat the random number generation for the specified count.
### Step 8:
Print each generated random number.
### Step 9:
End the program.

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
 for(int i = 0; i < count; i++) 
 {
 int random_number = (rand() % (max - min + 1)) + min;
 printf("%d\n", random_number);
 }
 return 0;
}
```

## OUTPUT:
![image](https://github.com/user-attachments/assets/db242d6d-e0fd-44f9-9f97-180fe1ad2660)

## RESULT:
The program is executed successfully.



