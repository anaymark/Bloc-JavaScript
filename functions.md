# Describe/define DRY and why functions exist.

* Dry is the acronym for Don't Repeat Yourself, means you should break code into components and have definition for a single responsibility, by creating functions for every single use.

# Describe/define the difference between creating a function and calling/executing a function.

* Creating a function means declaring a function, setting the parameters (if any), and entering the code of the function bloc. 

* Calling/executing a function is utilizing an instance of the function with or without parameters to do something or return something. Function can also be passed to other functions.  

 
# Describe/define what arguments/parameters are and how they relate to functions.

* Arguments/parameters are inputs that we pass into functions that behave like local variables. Parameters are needed for funtions to be able to take any input. 

# Describe/define mutating (dirty) vs non-mutating (pure) functions. 

* Mutating functions are those that change the existing object or data strucutre that they are called on directly. 

* Non-mutating functions are ones that produce a new object or data structure when they are called. 


```
var shoppingCart = [
  {
      id: 0,
      name: 'Mens Shirt',
      price: 20,
      size: 'Large'
  },
  {
  id: 1,
  name: 'kids shirt',
  price: 15,
  size: 'small'
}
]
function getTotalCost(items){
  let total = 0;
  // code below
  for (i=0;i<shoppingCart.length;i++)
    {
total += shoppingCart[i].price;
    }
  // code above
 return total;
}

getTotalCost(shoppingCart);

```