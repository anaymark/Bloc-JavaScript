# Describe a map method.
>Map method allows to create a new array and set it equal to an array that is iterated over every element with a defined function.

# Describe a filter method.
>Filter method allows to span an array and use a condition to include/exclude elements based on the given condition. The elements remaining will be the ones that return true with the given condition.

# What is the difference between a map and filter method?
>The map filter allows application of a function to all elements of an array to write to/create a new array. Whereas, the filter method allows to iterate through an array with a set condition and sort out the elements that do not return true to the defined condition.

```
var numbers = [1,2,3,4,5,6,7,8,9,2,3,4,5,6,1,2,3,4,5,6,7,8,8,4,3,2];

var red = numbers
.filter(num => num > 4)
//Filters out all number less than 4
.reduce((sum,num) => { return sum + num;});
//returns sum=80

```