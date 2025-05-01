# ⭐ Controlling Flow JS
In JavaScript, control flow is the order in which statements are executed.  Think of it as the "path" the JavaScript interpreter takes as it runs your code.  Normally, code executes sequentially, from top to bottom. However, control flow statements allow us to change this default behavior, enabling us to write more dynamic and complex programs.

## Conditional Statements
Allow you to perform various actions based on various 
conditions. 

### if ... else statements 
The if and else statements evaluate and expression and then run one block of code if the expression is truthy and another block of code if it's falsy. 

#### Ternary Operator
- A ternary operator is a concise way to express a conditional if ... else statements in one line of code.
    - The Ternary operator can only be used with two conditions

if ... else 

```javascript
let isNightTime = true;

if (isNightTime) {
  console.log('Turn on the lights!');
} else {
  console.log('Turn off the lights!');
}
```

  Ternary Operator 

```javascript
let isNightTime = true;
isNightTime ? console.log('Turn on the lights!') : console.log('Turn off the lights!');
```

#### Switch Statements
If your code needs to decide between more than two outcomes, use **switch statements**.

```javascript
switch(expression){
  case x:
    // code to run when expression === x
    break;
  case y:
    // code to run when expression === y
    break;
  default:
    // code to run if nothing else matches expression
 }
 ```


 ### Making Loops 

 Imagine that you want to write a program to count to 100 and output each number 
to the browser console. One way (one very tedious and inefficient way, I should 
say) would be to write 101 statements, like this:

prefix notation
The ++ operator before the variable (x) first increments the value of x by 1, and then returns the incremented value.
 ```javascript
 let x = 0;
 console.log(++x);
 console.log(++x);
 console.log(++x);
 console.log(++x);
 output: 1,2,3,4
 ```
 postfix notation
   The ++ operator after the variable (x) first returns the current value of x, and then increments the value of x by 1.
  ```javascript
 let x = 0;
 console.log(x++);
 console.log(x++);
 console.log(x++);
 console.log(x++);
 output: 0,1,2,3
 ```

  To make repeating statements easier, JavaScript provides several different types of looping statements, including these:

  - for
  The for loop is usually used to loop over code a predetermined number of times. 
  Uses initialization, condition, and final expression to loop. 
  Example: A for loop to do the counting to 100
  ```javascript 
  for(let i=1; i <= 100; ++i) {
  console.log(i); }
  ```
### for ... in 
  The for ... in loop iterates over the properties of an object and the properties it 
inherits from its parent object. B
### for ... of 
  The for ... of loop creates a loop by iterating over any iterable object. What's an iterable object, you ask? An iterable object is an object that can be iterated over. 
  Examples of iterable objects include arrays and strings.
  Example:

 ```javascript 
  const pets = ['cat', 'dog', 'chicken'];
 for (let pet of pets) {
  console.log(pet);
  output: 
  cat 
  dog 
  chicken
 }
  ```

  ```javascript
   let text = "mom";
 for (let character of text) {
  console.log(character);
 }

output:
m 
o 
m 

  ```
### do ... while 

The do...while loop executes the code block at least once, and then it evaluates the condition.This means the code block inside a do...while loop will always run at least one time, regardless of the initial state of the condition.
**"Do this at least once, and continue doing it as long as this condition is true."**
    - Use when you need to check a condition before potentially executing a code. 
### while

The while loop evaluates its condition before executing the code block inside the loop.If the condition is initially false, the code block within the while loop will never be executed.
  - Use when you need to guarantee that a block of code runs at least once, even if the condition is initially false. 
  - Presenting a menu to a user and ensuring they see it at least once before a condition (like choosing to exit) is checked.
  - Implementing input validation where you want to prompt the user for input at least once before checking if it's valid.

### break and continue statements 
The break and continue statements can be used to interrupt the execution of a loops 

- *Break* causes the current loop or control statement to exit. 
- *Continue* halts execution of the current iteration of the loop and goes directly to the next one. 
``` javascript
let phoneNumber = "555-757-1212";
 for (let digit of phoneNumber) {
  if (digit==='-') continue;
  console.log(digit);
 }
```