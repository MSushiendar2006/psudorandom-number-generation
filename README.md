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
Developed By:Sushiendar M
Registration Number:212223040217
```
```
#include <stdio.h>
//Constants for LCG
#define A 1664525
#define C 1013904223
#define M 4294967296 // 2^32

//Linear Congruential Generator function
unsigned int lcg(unsigned int seed) {
    return (A * seed + C) % M;
}

int main() {
    unsigned int seed;
    int n, i;
    printf("*Pseudorandom number generator*\n\n");
    printf("Enter the seed value: ");
    scanf("%u", &seed);
    printf("Enter how many random numbers to generate: ");
    scanf("%d", &n);
    printf("Random numbers:\n");
    for (i = 0; i < n; i++) {
        seed = lcg(seed);
        printf("%u\n", seed);
    }
    return 0;
}
```
## OUTPUT:
![image](https://github.com/user-attachments/assets/4d2ffc12-ac20-42dd-a8a2-9881813d970b)

## RESULT:
The program is executed successfully.





