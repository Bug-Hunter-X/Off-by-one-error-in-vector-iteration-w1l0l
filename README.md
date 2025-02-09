# Off-by-One Error in Vector Iteration

This repository demonstrates a common off-by-one error in C++ when iterating over a `std::vector`.  The error arises from using `<=` in the loop condition instead of `<`, resulting in accessing an element outside the valid range of the vector.

## Bug Description

The `bug.cpp` file contains a simple program that iterates over a vector.  Due to the incorrect loop condition, it attempts to access an element beyond the vector's last element, causing undefined behavior (likely a crash or unpredictable output). 

## Solution

The `bugSolution.cpp` file provides a corrected version with the loop condition fixed to use `<` instead of `<=`. This ensures that the loop only iterates through valid indices within the vector.