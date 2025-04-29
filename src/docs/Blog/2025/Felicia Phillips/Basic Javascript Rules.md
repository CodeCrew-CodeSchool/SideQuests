## ⭐ Basic Javascript


### Funcation declaration 

A function declaration is a function that is bound to an identifier, or name. 

function declaration example:

```javascript
function identifier() {
 //statements or instructions that are executed by the browser
}
```

Calling function 

```javascript 
identifier();
```

This function call executes the function body, or all of the statements between the curly braces in the function declaration.



### Default Parameters 

 Default parameters allow parameters to have a predetermined value in case there is no argument passed into the function or if the argument is undefined when called.


```javascript
 function greeting (name = 'stranger') {
  console.log(`Hello, ${name}!`)
}

greeting('Nick') // Output: Hello, Nick!
greeting() // Output: Hello, stranger!


```

To pass back information from the function call, we use a return statement.


## Different ways to write a function in JavaScript

### 1. Function Declaration
```javascript
function hello() {
  console.log("Hello");
}
```

### 2. Function Expression
```javascript
const helloAgain = function() {
  console.log("Hello again!");
};
```
### 3. Arrow Function
```javascript
const helloWorld = () => console.log("Hello World");
```

### 4. Arrow Function (Template Literals)
```javascript

(parameters) => some code

```javascript
setTimeout(() => console.log("Aye Mane one more time!"), 3000);
```
Key Takeaway:  setTimeout schedules a function to run *later*, without blocking other code.

## Higher Order Arrow Functions

```javascript
const numbers = [1,2,3,4,5,6];
const square = numbers.map((element) => Math.pow(element,2));
const cube = numbers.map((element) => Math.pow(element,3));
const evenNums = numbers.filter((element) => Math.pow element % === 0);

//example #2

const helloName = (name) => {
  console.log(`Hello ${name}`);

  // Explanation:
  // -  Takes one argument: 'name'.
  // -  Uses a template literal (backticks ``).
  // -  `${name}` is interpolation, inserting the 'name' value.
  // -  No curly braces needed for a single statement.
};
```

## Function Calls
```javascript
hello();
helloAgain();
helloWorld();
helloName("Collierville");
```

## setTimeout Example (Asynchronous Execution) Example

setTimeout(callback, delayInMs);  

Syntax: Function to call, delay in milliseconds

Executes a function *after* the specified delay (in milliseconds).

### Named Function Callback
```javascript
function helloMemphis() {
  console.log("Aye Mane");
}
setTimeout(helloMemphis, 3000);  // Logs "Aye Mane" after 3 seconds.
```

### Anonymous Function Callback
```javascript
setTimeout(function() {
  console.log("Aye Mane again!");
}, 3000);
```