# Off-by-One Error in Java Array Iteration

This repository demonstrates a common off-by-one error in Java when iterating through arrays. The code attempts to access an element beyond the array's valid index range, resulting in an `ArrayIndexOutOfBoundsException`.  The solution provides a corrected version with proper loop bounds.

The problem arises from the loop condition `i <= arr.length`.  Arrays in Java are zero-indexed, meaning the valid indices are from 0 to `arr.length - 1`.  The incorrect condition tries to access `arr[arr.length]`, which is out of bounds.

The solution adjusts the loop condition to `i < arr.length`, ensuring that the loop terminates before accessing an invalid index.