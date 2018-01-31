# What does "lexical scope" mean in JavaScript?
> Lexical scope in javascript eludes to the fact that variables defined withing blocs of code may only be referenced from within the defined block of code. Meaning variables defined within functions or objects exist in the local instance of that saif function or object. However, this also means variables can be defined in a global manner or a child function/object will have access to the variables of the parent. 


# What is an advantage of a programming language that uses lexical scoping?
> The advantage of lexical scoping is that local variables can be defined to a code block that do not interfere with global variables and do not create naming conflicts. Moreover, the variables that are defined within a function are only stored in memory when the said function is called and executes, upon finishing execution the variabes are wiped from memory. 


# What is a closure?
>Closures are any functions that use a variable outside of it's scope. These functions preserve data, in the sense that they have access to the outer/parents functions variables and parameters. These functions can also manipulate the variables of the outer/parent functions. 



# What would be a use case of a closure?
>One of the most useful cases for closures is to create a private function, since this ability is not defined in javascript. Closures allow to emulate this, which is known as the module pattern.

JS 
```
var codeSalary = (function() {
 var salary = 70000;
 function changeBy(amount){
   salary += amount;
 }
  return{
    raise: function()     {
      changeBy(10000);
    },
    lower: function()
    {
          changeBy(-10000);
    },
    currentSalary: function (){
      return salary;
    }
  };
})();
  
                  
```

>This is an example of something we want to keep as a private variable or only within this code block/function. The salary can be changed through accessing raise, lower or currentSalary, but cannot be accessed directly. The salary is not defined since we have it as a local variable to the said function. 

```
codeSalary.lower()
//undefined

codeSalary.currentSalary()
// 60000

console.log(salary)
//salary not defined            
                  
```
