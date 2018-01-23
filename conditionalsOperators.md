# What are the three types of conditional statements?

* if

* else if

* else


# What are four types of Comparison Operators and how you would use them?

* == equality operator, used to compare two data values and return true or false based on data values.

* === strict equality operator, used to compare two data values as well as the data type at question, returns true or false based on both data values and data types.

* != inequality operator, used to compare two data values and return true or false based on inequality of data value. 

* !== strict inequality operator, used to compare two data values as well as data types at question, returns true or false based on both data values and data types. 

* > greater than, compares two data values, and returns true or false based on value comparison. non-inclusive.

* < less than, compares two data values, and returns true or false based on value comparison, non-inclusive.

* >= greater than or equal to, compares two data values, and returns true or false based on value comparison, inclusive. 

* <= less than or equal to, compares two data values, and returns true or false based on value comparison, inclusive.

* && logical and operator, all coditions have to be true to return a true value, all other scenarios will return false.

* || logical or operator, any of the conditions must be true to return true. However, if the first operator is true, the second operator will not be checked. 


```

// add code here
var grade = "A";

if (grade === "A"){    console.log("Congrats you have passed!!!");
  }
else if (grade === "B"){
  console.log("Congrats you have passed, but not perfect.");
}
else if (grade === "C"){
  console.log("You passed, barely...");
}
else if (grade === "D"){
  console.log("You failed!");
}
else if (grade === "F"){
  console.log("Try Again!")
  }
else 
  {
  console.log("Not sure what happend.")
  }

```
