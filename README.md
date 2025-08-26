# task-1-circular-array-path
Circular Array Path Generator

A Java solution for generating paths in circular arrays by moving with a fixed interval length. This program processes two circular arrays simultaneously and combines their results into a single path.

Problem Description

Given two circular arrays (each defined by size n and step m), the program calculates the path formed by starting at the first element and moving in steps of length m. After reaching the end of the array, it continues from the beginning (circular behavior). The path consists of the starting elements of each interval.
Mathematical Foundation

The solution utilizes modular arithmetic to efficiently navigate circular arrays without physically creating them. The key formula for calculating the next starting element is:

next = (current + m - 1) % n
if (next == 0) next = n

This approach ensures optimal performance even for large values of n.

Algorithm Explanation

  1.  For each circular array, start at the first element (1)
  2.  Add the current element to the path
  3.  Calculate the next starting element using modular arithmetic
  4.  Repeat until returning to the first element
  5.  Combine paths from both arrays into the final result
