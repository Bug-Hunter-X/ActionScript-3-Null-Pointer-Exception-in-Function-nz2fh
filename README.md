# ActionScript 3 Null Pointer Exception

This repository demonstrates a common ActionScript 3 bug involving unexpected null pointer exceptions within functions.  The variable `someVariable` becomes null unexpectedly, causing the `trace` statement to fail and the program to crash.

## Bug Description

The `myFunction` attempts to access and trace the value of `someVariable`. Under certain conditions, `someVariable` might be null leading to a runtime `NullPointerException`. The exact circumstances causing this null value are not obvious in this simplified example but might involve complex event handling or asynchronous operations in a larger application.

## Solution

The solution requires identifying the root cause of the `someVariable` becoming null.  Appropriate null checks and error handling should be implemented to prevent the `NullPointerException`. The example demonstrates a solution using an if condition to handle the case where the variable is null before using it.

## How to reproduce

1. Compile the code in the `bug.as` file. 
2. Run the application in a suitable ActionScript 3 runtime environment (e.g., Flash Player, AIR).
3. Observe the runtime exception when `someVariable` is null. 