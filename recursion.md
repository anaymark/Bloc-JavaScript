# What is recursion?
> Recursion is a technique for iterating using an operation by a function self-calling over and over until the defined result/parameter is reached.


# When would a programmer want to write a recursive function instead of an iterative one?
> Recursive functions are reserved for a problem that is difficult to implement using an iterative function, a problem that consists of many subproblems. Recursion is also a useful method for transversing the DOM and setting up a leave event.

# What is a base case and what is its role in a recursive function?
> A base case is a case that is used to terminate the function and exit the recursive loop. Base cases are also useful to define cases that cannot be reached from logical code. 


# What would happen if a programmer did not utilize a base case within a recursive function?
> The function would most likely become an infinite function and/or not reach certain cases that are unreachable by logic. 

```
// add code below
function factorial(n) {
  if (n === 0) {
    return 1;
  }
  return n * factorial(n - 1);
}

```