# What is object-oriented programming?
>OOP defines the concept of objects modeling real things and being able to interact through the use of methods(functions) and attributes(variables). The idea of inheritance is a large driver of OOP in which classes or parent objects give instances to child objects and relay the acess to methods and variables within the parents scope. There is also the concepts of abstraction and encapsulation in OOP, in such that objects only reveal the necessary data, allowing software interaction to be secure and simple. 


# What is a constructor?
> Constructor is a special method for creating instances of an object that was defined with class. This further relays the idea of inheritance. Constructors allow for inheritance of attributes and really save time in defining a parent object that can instantiate multiple objects from it's blueprint. 


# What is the purpose of the keyword super?
> Super is the keyword that allows an extended class to access the parent constructor.

# What are classes that do not use the keyword extends called?
> Classes that do not use the extends keyword are the constructor classes, the classes that will be used as the parent. 


```
var Clothes = class {
    constructor(name, size, price){
        this.name = name;
        this.size = size;
        this.price = price;
    }
}

// add code below

class Shirt extends Clothes {
  constructor(){
    super('Designer','XXL',50)
  }
}

```