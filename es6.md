# What does "DRY" stand for? What does the "DRY principle" imply in programming or software development?
> Dry is the acronym for "do not repeat yourself". This prinicple is especially important in software develoment, the goal is to define every single responsibility to a single block of code. This idea is represented best with inheritance and extendability of classes. The ability to define a class prototype and build multiple extended classes is what the DRY principle is all about. 

```
// add code below
class Product {
  constructor (name,size,price) {
    this.name = name;
    this.size = size;
    this.price = price;
  }
  getName(){
    return this.name
  }
  getSize(){
    return this.size
  }
  getPrice(){
    return this.price
  }
}

class Shirt extends Product {
  constructor(){
    super('shirt','XXL',55)
  }
  
  getName() {
    return "You've selected a " + super.getName();
  }
  
  getSize() {
    return "The size you've selected is: " + super.getSize();
  }
  
  getPrice() {
    return "The cost of the " + super.getName() + "is " + super.getPrice();
  }
}

class Jacket extends Product {
  constructor() {
    super('jacket','XXL',155)
  }
 
    getName() {
    return "You've selected a " + super.getName();
  }
  
  getSize() {
    return "The size you've selected is: " + super.getSize();
  }
  
  getPrice() {
    return "The cost of the " + super.getName() + "is " + super.getPrice();
  }
}

class Scarf extends Product {
  constructor(){
    super('scarf','XL',200)
  }
 
    getName() {
    return "You've selected a " + super.getName();
  }
  
  getSize() {
    return "The size you've selected is: " + super.getSize();
  }
  
  getPrice() {
    return "The cost of the " + super.getName() + "is " + super.getPrice();
  }
}

let shirt = new Shirt();

shirt.getName();
shirt.getSize();
shirt.getPrice();

let jacket = new Jacket();

jacket.getName();
jacket.getSize();
jacket.getPrice();

let scarf = new Scarf();

scarf.getName();
scarf.getSize();
scarf.getPrice();

```