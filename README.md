# Goldbach’s Conjecture in Array
Implement functions to initialize an array with random natural numbers, determine prime numbers, and find Goldbach's pair for even numbers greater than 4 in the array.

## Introduction:
Goldbach’s conjecture, named after German mathematician Christian Goldbach on June 7, 1742, is a problem that states any even positive integer greater than four (4) can be expressed as the sum of two odd prime integers. For example:
10 = 5 + 5, 3 + 7

Although this conjecture holds true up to 4 x 10^18, it remains unproven that all even positive integers above 4 have a Goldbach partition. Therefore, it stands as one of the best-known unsolved problems in number theory and mathematics, remaining open for proof for more than 200 years.

## Learning Outcomes:
- Implement an initialization of the array with random natural numbers.
- Implement a function to print the Goldbach’s pair of an even natural number greater than 4 in the array.

## Problem Description:
1. `void initArrayRandInt(int x[], int s);`
   - Initializes array `x` of size `s` with random positive integers.

2. `bool isPrime(int x);`
   - Determines if integer `x` is a prime number.
   - Return 1 if `x` is prime, 0 otherwise.

3. `bool isEven(int x);`
   - Determines if integer `x` is an even number greater than 4.
   - Return 1 if `x` is even, 0 otherwise.

4. `void printGoldbachsPairInArray(int x[], int s);`
   - Prints the Goldbach’s pair (1 pair only) of element(s) in the array (if there are any).
   - Uses the `isPrime` and `isEven` functions.

## Usage:
Call the `printGoldbachsPairInArray` function from the `main` function after initializing the array with random natural numbers using `initArrayRandInt`. This will display the Goldbach's pair for the even elements in the array (if there are any).

```c
#include <stdio.h>
#include <stdlib.h>
#include <time.h>

// Function prototypes (definitions are provided in the implementation)
void initArrayRandInt(int x[], int s);
bool isPrime(int x);
bool isEven(int x);
void printGoldbachsPairInArray(int x[], int s);

int main() {
    // Set a seed for random number generation
    srand(time(0));

    // Define the size of the array
    const int size = 10;
    
    // Create an array of size 'size'
    int array[size];

    // Initialize the array with random positive integers
    initArrayRandInt(array, size);

    // Print the Goldbach's pair for the even elements in the array
    printGoldbachsPairInArray(array, size);

    return 0;
}
```

## How to Contribute:
Contributions to this project are welcome! If you have any suggestions, bug fixes, or improvements, please follow these steps:
1. Fork this repository.
2. Create a new branch with a descriptive name.
3. Make your changes and commit them with clear commit messages.
4. Push your changes to your forked repository.
5. Submit a pull request explaining the changes you've made.

## Credits:
This problem was presented as a C++ Lab Exercise by Sir Michael Jay Anthony Regis. 

## License:
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more details.
