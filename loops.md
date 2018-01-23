# What are the three things you need to provide for a loop? I.e. for(a; b; c;), what are a, b, and c?

* a-initialization: set initial value for the iterator variable

* b-condition: the condition that must be met before the loop will terminate.

* c-final-expression: the increments for loop iteration. 

# Describe infinite loops and how to avoid them.

>Infinite loops occur when a condition is set that can never be reached, or a condition that is always true occurs (ie. no change). Either one can be avoided by checking logic of setting up the loops. 

```
for (i = 0; i < shoppingCart.length; i++)
  {
console.log(shoppingCart[i]);
  }
```