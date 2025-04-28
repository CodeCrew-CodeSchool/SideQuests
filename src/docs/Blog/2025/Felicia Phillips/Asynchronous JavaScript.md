# ⭐ Asynchronous JavaScript

Synchronous: Executes code line by line consecutively in a sequential manner. Basically code that waits for an operation to complete. 
Asynchronous: Allows multiple operations to be perfromed concurrently without waiting.
example:
```javascript 
setTimeout(()=> console.log("Task 1"), 3000) 
console.log("Task 2");
console.log("Task 3");
console.log("Task 4");
```
## Three Types of Asynchronous 
- Callbacks is a function that is passed as an argument to another function. 
Used to handle:
1. Reading a file.
We could use a callback to instruct javascript to display content after we are done reading the file. 
2. Network requests.
4. Fetching data from a server
5. Setting a timer
 "Hey, do this task, and when you're done, call this other function for me."

 ⭐ Analogy:

 Imagine you go to a restaurant and order food. You don't just stand there and wait for your meal to be prepared. Instead, you give your order (the callback) to the waiter (the other function), and you go sit down. The waiter (the other function) takes your order to the kitchen (the asynchronous operation). Once your food is ready (the operation is complete), the waiter calls you back (executes your callback) to let you know.

 OR 

 Imagine ordering food at a restaurant. Your order (the callback) tells the waiter (JavaScript) what to do when the food is ready. The waiter, busy with other tables (other tasks), gives your order to the kitchen (the asynchronous operation). Once prepared, the waiter, when available, brings you the food (executes the callback). This shows how JavaScript handles tasks concurrently, executing your instructions only after the background work is complete.


⭐ Example:
```javascript

hello(wait);
goodbye();

function hello(callback){
    console.log("Hello");
    callback();
}

function leave(){
    conole.log(Leave)
}

function wait(){
    console.log(wait)
}

function goodbye(){
    console.log("Goodbye!")
}

//by using callbacks, we are guarantrring that the function passed in will execute next.

example 2 
function sum(callback, x, y){
    let result = x+y;
    callback();
}

function displayConsole(result){
    console.log(result);
}
```
- Promises:
- Async/Await: