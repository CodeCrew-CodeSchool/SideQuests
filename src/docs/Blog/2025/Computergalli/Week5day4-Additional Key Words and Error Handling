Understanding for Loops in JavaScript
Overview
The for loop is a fundamental feature in JavaScript that allows you to repeat a block of code a specific number of times. It is especially useful when you know in advance how many times you want to execute a piece of code.

What is a for Loop?
A for loop repeats a block of code as long as a specified condition is true. It's most commonly used when the number of repetitions is known beforehand.

Basic Syntax
for (initialization; condition; iteration) {
  // Code to execute each time the loop runs
}
Initialization: This step sets up a loop control variable, usually starting at a particular value.
Condition: This expression is checked before each loop iteration. If the condition is true, the loop continues; if false, the loop stops.
Iteration: After each loop iteration, this expression updates the loop control variable, usually by incrementing or decrementing it.
Example: Counting to 5
for (let i = 1; i <= 5; i++) {
  console.log("Count is: " + i);
}
Explanation:

Initialization: let i = 1; initializes the counter i at 1.
Condition: i <= 5 checks if i is less than or equal to 5. If true, the loop continues; if false, the loop stops.
Iteration: i++ increments i by 1 after each loop iteration.
The loop prints "Count is: X" where X is the current value of i, and stops when i exceeds 5.
Counting Down
You can also use a for loop to count down by changing the initialization, condition, and iteration accordingly.

Example: Counting Down from 5 to 1
for (let i = 5; i >= 1; i--) {
  console.log("Count is: " + i);
}
Explanation:

Initialization: let i = 5; initializes the counter i at 5.
Condition: i >= 1 checks if i is greater than or equal to 1. If true, the loop continues; if false, the loop stops.
Iteration: i-- decrements i by 1 after each loop iteration.
The loop prints "Count is: X" where X is the current value of i, and stops when i becomes less than 1.
Conclusion
The for loop is a versatile feature that allows you to repeat a block of code a specific number of times. By setting up the initialization, condition, and iteration correctly, you can control exactly how many times the loop runs, making it a powerful tool in your programming toolkit.

In functions, we can return the value of the function by using the keyword “RETURN”. When we use the return statement in a function it’s the execution of the entire function. Which means the other code that is written after the return statement is not going to work.

Example:

function sum(num1, num2) {
  return num1 + num2;
}
let result = sum(1, 2);
console.log(result); // 3
 

The break statement breaks out of a switch or a loop. In a switch, it breaks out of the switch block. This stops the execution of more code inside the switch. In in a loop, it breaks out of the loop and continues executing the code after the loop (if any).

Break out of a list:

let text = "";
const cars = ["BMW", "Volvo", "Saab", "Ford"];

list: {
  text += cars[0] + "<br>";
  text += cars[1] + "<br>";
  text += cars[2] + "<br>";
  break list;
  text += cars[3] + "<br>";
}
 

The continue statement breaks one iteration (in the loop), if a specified condition occurs, and continues with the next iteration in the loop.

This example skips the value of 3:

for (let i = 0; i < 10; i++) {

   if (i === 3) { continue; }

   text += "The number is " + i + "<br>";
   }
 

Error Handling

Try ... Catch : The try statement defines a code block to run (to try). The catch statement defines a code block to handle any error.

try {
  Block of code to try
}
catch(err) {
  Block of code to handle errors
}
Finally : The finally statement defines a code block to run regardless of the result. The finally block contains statements to be executed after the try and catch blocks execute. Additionally, the finally block executes before the code that follows the try…catch…finally statement.

try {
  Block of code to try
}
catch(err) {
  Block of code to handle errors
}
finally {
  Block of code to be executed regardless of the try / catch result
}
 

Throw : The throw statement defines a custom error. Technically you can throw an exception (throw an error). The exception can be a JavaScript String, a Number, a Boolean or an Object:

throw "Too big";    // throw a text
throw 500;          // throw a number
If you use throw together with try and catch, you can control program flow and generate custom error messages.

