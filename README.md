# Java ArrayIndexOutOfBoundsException Bug

This repository demonstrates a common Java programming error: an `ArrayIndexOutOfBoundsException`.  The provided `bug.java` file contains code that attempts to access an array element outside its valid index range, resulting in a runtime exception. The corrected code is in `bugSolution.java`.

## Bug Description
The `for` loop in `bug.java` uses an incorrect condition (`i <= arr.length`), causing the loop to iterate one time too many. This results in an attempt to access `arr[5]` in an array of size 5, resulting in the exception.

## Solution
The `bugSolution.java` file corrects this by changing the loop condition to `i < arr.length`.  This ensures that the loop only accesses valid array indices.

## How to run
1. Save `bug.java` and `bugSolution.java`
2. Compile each using a Java compiler: `javac bug.java` and `javac bugSolution.java`
3. Run each using a Java Virtual Machine: `java bug` and `java bugSolution`