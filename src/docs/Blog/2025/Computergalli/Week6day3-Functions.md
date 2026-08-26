In this lesson, students will learn the fundamentals of JavaScript functions. They will explore how to create functions, use built-in functions, and place functions within objects (methods). The lesson also covers the importance of functions in organizing and reusing code efficiently.

Learning Goals
Understand what a function is and its purpose in JavaScript.
Create and invoke their own functions.
Use built-in JavaScript functions effectively.
Place functions inside objects as methods.
Understand the difference between function declarations and expressions.
Success Criteria
Students can define and invoke custom functions.
Students can use common built-in JavaScript functions.
Students can attach functions as methods within objects and access them.
Students can explain the difference between function declarations and function expressions.
Definitions
Function: A block of reusable code designed to perform a specific task.
Function Declaration: A way to define a function with the function keyword followed by a name.
Function Expression: A function assigned to a variable.
Built-in Function: Predefined functions in JavaScript (e.g., Math.random(), parseInt(), alert()).
Method: A function that is a property of an object.
Parameter: A variable in the function definition that accepts input.
Argument: The actual value passed to the function when it is invoked.
Return Value: The value that a function gives back after execution.
 

Arrays Functions

 

Overview
The Map, Filter, and Reduce Array methods are few more useful tools that we will be exploring today.

 

Objectives
Learn how to effectively use map, filter, and reduce array methods to manipulate data, transform arrays, and perform computations. Understand their syntax, common use cases, and how they can simplify complex operations on arrays. By the end of this lesson, you’ll be equipped with powerful tools to enhance your array manipulation skills! 

Execute

Array Functions
The map() method is used for creating a new array from an existing one, applying a function to each one of the elements of the first array.
The filter() method takes each element in an array and it applies a conditional statement against it. If this conditional returns true, the element gets pushed to the output array. If the condition returns false, the element does not get pushed to the output array.
The reduce() method reduces an array of values down to just one value. To get the output value, it runs a reducer function on each element of the array.
Map/filter/reduce in a tweet:

map([🌽, 🐮, 🐔], cook)

=> [🍿, 🍔, 🍳]

filter([🍿, 🍔, 🍳], isVegetarian)

=> [🍿, 🍳]

reduce([🍿, 🍳], eat)

=> 💩
