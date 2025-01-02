# F# Mutable Variable Bug

This example demonstrates a common error related to mutable variables and function scope in F#.  The intention is to create a function to swap the values of two mutable variables. However, due to how F# handles variable scoping and references, the swap operation only affects the variables within the `swap` function's scope. The variables x and y in the main program remain unchanged.

## How to reproduce the bug
1. Copy and paste the code into an F# script or project.
2. Run the script or build/run the project. 
3. Observe that the output shows that the variables x and y are not swapped, demonstrating the unintended behavior.