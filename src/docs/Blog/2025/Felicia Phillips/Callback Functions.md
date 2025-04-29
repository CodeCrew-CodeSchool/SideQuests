## ⭐ What is a callback function ?


At its core, a callback function is a function that is passed as an argument to another function. The "calling" function is expected to execute this callback function at some point during its own execution. Think of it as saying, **"Hey, I'm going to do some work, and when I'm done (or at a specific point), please run this function for me."**


## Usages

### Asynchronous Operations
When used in asynchronous operations, such as reading a file, making a network request, setting a timer, callbacks provide a way to execute code after the asynchronous operation has completed.


```javascript
function fetchData(url, callback) {
  console.log(`Fetching data from ${url}...`);
  // Simulate an asynchronous operation with setTimeout
  setTimeout(() => {
    const data = { message: "Data fetched successfully!" };
    callback(null, data); // Call the callback with the result
  }, 2000);
}

function processData(error, result) {
  if (error) {
    console.error("Error:", error);
    return;
  }
  console.log("Data:", result.message);
}

fetchData("https://example.com/api/data", processData);
console.log("Fetching initiated..."); // This line executes immediately
```



### Higher-Order Functions

Higher-Order Functions: Functions that operate on other functions, either by taking them as arguments or returning them, are called higher-order functions. 1  Methods like .map(), .filter(), .reduce(), .forEach() in JavaScript are excellent examples. They use callbacks to apply custom logic to each element of an array.

``` javascript
const numbers = [1, 2, 3, 4, 5, 6];

const square = (element) => Math.pow(element, 2);
const cube = (element) => Math.pow(element, 3);
const isEven = (element) => element % 2 === 0;

const squares = numbers.map(square);
const cubes = numbers.map(cube);
const evenNums = numbers.filter(isEven);
```

### Event Handling
Event Handling: In user interfaces and event-driven systems, callbacks are used to define what should happen when a specific event occurs (e.g., a button click, a mouseover, a keypress).

```javascript
document.getElementById('myButton').addEventListener('click', function() {
  console.log('Button clicked!');
});
```