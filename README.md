# Improper Error Handling in JavaScript Calculator

This repository demonstrates a common error in JavaScript: improper error handling in a simple calculator function. The `calculate` function uses a `switch` statement to perform different arithmetic operations based on the operator provided by the user. However, it does not gracefully handle potential errors, such as division by zero. 

## Bug

The `divide` function correctly throws an error when attempting to divide by zero. However, the `calculate` function does not catch this error. If a zero is provided as the divisor, the program will terminate abruptly with an unhandled exception. This is a poor user experience. 

## Solution

The solution demonstrates how to improve this error handling using `try...catch` blocks. The solution adds a `try...catch` block to the `calculate` function to catch potential errors during the calculation and return an error message instead of crashing the program. This makes the application more robust and prevents unexpected terminations. 