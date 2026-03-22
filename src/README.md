# Assignment 1: Recursion
**Name:** [Nurali Amangeldi]
**Group:** [IT-2504]

## Work Process Summary
[cite_start]In this assignment, I implemented 10 recursive functions in Java without using any loops (for, while). 
[cite_start]Each solution focuses on a base case to stop recursion and a recursive step to solve the problem.


---

## Part 1: Numbers

### Task 1: Print Digits
*Output check:*
![Task 1 Screen](../screens/task1.png)

### Task 2: Average of Elements
*Output check:*
![Task 2 Screen](../screens/task2.png)

### Task 3: Prime Number Check
*Output check:*
![Task 3 Screen](../screens/task3.png)

### Task 4: Factorial
*Output check:*
![Task 4 Screen](../screens/task4.png)

---

## Part 2: Sequences

### Task 5: Fibonacci Number
*Output check:*
![Task 5 Screen](../screens/task5.png)

### Task 6: Power Function
*Output check:*
![Task 6 Screen](../screens/task6.png)

### Task 7: Reverse Output
*Output check:*
![Task 7 Screen](../screens/task7.png)

---

## Part 3: Strings and GCD

### Task 8: Check Digits in String
*Output check:*
![Task 8 Screen](../screens/task8.png)

### Task 9: Count Characters
*Output check:*
![Task 9 Screen](../screens/task9.png)

### Task 10: Greatest Common Divisor
*Output check:*
![Task 10 Screen](../screens/task10.png)

Task 1: Digit Extraction
Description: A function that takes an integer and prints every digit on a separate line.
Logic: The function calls itself with n divided by 10 to reach the first digit, then prints the remainder after the recursion returns to ensure the correct order.


Task 2: Recursive Array Processing
Description: Functions to fill an array with user input and calculate the average value of its elements.
Logic: The fill function moves through array indices to store input, while the sum function adds the current element to the sum of the remaining elements.

Task 3: Primality Test
Description: A recursive function to check if a positive integer n is a prime number.
Logic: The function tries to divide n by an incrementing divisor starting from 2. If n is divisible by any number before reaching the limit, it is Composite; otherwise, it is Prime.


Task 4: Factorial Calculation
Description: Calculates the factorial of a given number n.
Logic: It uses the formula n multiplied by the factorial of (n minus 1) until the base case of 1 is reached.

Part 2: Sequences and Math 
Task 5: Fibonacci Sequence Description: Finds the n-th number in the Fibonacci sequence.
Logic: The function adds the two previous Fibonacci numbers together using the base cases where F(0) is 0 and F(1) is 1.
Task 6: Power Function Description: Calculates a number a raised to the power of n.
Logic: The function multiplies a by the result of the power function with the exponent decreased by 1 until the exponent reaches 0.
Task 7: Recursive Reversal Description: Reads n integers and prints them in reverse order without using another array.
Logic: The function reads a number, calls itself for the next numbers, and then prints the current number after the recursive call returns.
Part 3: Strings and Advanced Math

Task 8: Digit Validation
Description: Checks if a string consists only of digits.
Logic: It checks the first character; if it is a digit, it calls itself with the rest of the string. It returns No if any non-digit is found.
Task 9: Count Characters
Description: A recursive function that counts the total number of characters in a given string.
Logic: The function returns 1 plus the count of the remaining substring until the string is empty.

Task 10: Greatest Common Divisor
Description: Finds the GCD of two numbers using the Euclidean Algorithm.
Logic: The function repeatedly takes the remainder of the two numbers until the second number becomes 0.