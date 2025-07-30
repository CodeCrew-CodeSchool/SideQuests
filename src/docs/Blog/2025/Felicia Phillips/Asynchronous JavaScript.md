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

### Callbacks
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

//by using callbacks, we are guaranteeing that the function passed in will execute next.

example 2 
function sum(callback, x, y){
    let result = x+y;
    callback();
}

function displayConsole(result){
    console.log(result);
}
```

### Promises
- Promises: A Promise is an object that acts as a placeholder for the eventual result of an asynchronous operation. It represents a value that might not be available immediately.

⭐ Think of it like this: 
- You place your order (the asynchronous operation is initiated).
- You get a ticket with your order number (the Promise object).
- While your food is being prepared, you can do other things (your program can continue executing other code).
- Eventually, your order is ready (the asynchronous operation completes), and you are notified (the Promise resolves with the result, or rejects if there was an error).

⭐ Usage: 

- Fetching data from a server (using APIs).
- Reading or writing files.
- Setting timers (like setTimeout).
- User interactions (like clicks, but Promises are not the primary way to handle these directly).

⭐ States of a Promise
- Pending: This is the intial state. 
- Fulfilled(Resolved): It completed successfully.
- Rejected: It has failed.

example:
//Do these chors in order 
1. Walk the dog 
2. Clean the kitchen
3. Take out the trash

```javascript

/* Step 1: Create the functions
function walkDog(){
    setTimeout(() => {
        console.log("You walk the dog");
    } ,1500)
}

function cleanKitchen(){
    setTimeout(() => {
        console.log("You clean the kitchen");
    } ,2500)
}

function takeOutTrash(){
    setTimeout(() => {
        console.log("You take out the trash");
    } ,500)
}
*/

Step 2: use callbacks to execute these chores in order
function walkDog(callback){
    setTimeout(() => {
        console.log("You walk the dog");
        callback(); //after the code is complete we will evoke the callback
    } ,1500)
}

function cleanKitchen(callback){
    setTimeout(() => {
        console.log("You clean the kitchen");
        callback();
    } ,2500)
}

function takeOutTrash(callback){
    setTimeout(() => {
        console.log("You take out the trash");
        callback();
    } ,500)
}

3. Callback Hell 

walkDog( () => {
    cleanKitchen(() => {
        takeOutTrash (() => console.log("Done!"))
    });
});

Promise 

Step 2: use callbacks to execute these chores in order
function walkDog(){

    return new Promise ((resolve, reject) => {
  setTimeout(() => {
        resolve("You walk the dog");
    } ,1500)

    });
}

function cleanKitchen(){

    return new Promise ((resolve, reject) => {
  setTimeout(() => {
        resolve("You clean the kitchen");
    } ,2500)

    });
}


function takeOutTrash(){

    return new Promise ((resolve, reject) => {
  setTimeout(() => {
        resolve("You take out the trash");
    } ,500)

    });
}

//method chaining 
walkDog().then(value= =>{console.log(value); return cleanKitchen()})
         .then(value => {console.log(value); return takeOutTrash()})
         .then(value => {console.log(value); console.log("You're finished")});

```

- Async/Await: