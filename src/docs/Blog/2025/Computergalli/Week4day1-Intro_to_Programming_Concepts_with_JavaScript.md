JavaScript is a versatile and powerful programming language that adds interactivity and dynamism to web pages.
it enables developers to create interactive features, validate forms, manipulate the Document Object Model (DOM), and handle user interactions.


const myHeading = document.querySelector("h1");
myHeading.textContent = "Hello world!";
let myVariable;

JavaScript Variable Types
1. String
A sequence of text.
Must be enclosed in single (' ') or double (" ") quotes.
Example:

let myVariable = 'Bob'; 
let myVariable = "Bob";
2. Number
Represents numerical values.
No quotes needed.
Example:


let myVariable = 10;
3. Boolean
Represents true or false values.
Used for logical operations.
No quotes needed.

Example:
let myVariable = true;
4. Array
A collection of multiple values stored in a single reference.
Values can be of different types.
Access elements using index notation (myVariable[index]).

Example:
let myVariable = [1, 'Bob', 'Steve', 10];
console.log(myVariable[0]); // Output: 1
console.log(myVariable[1]); // Output: 'Bob'
5. Object
Can represent anything (everything in JavaScript is an object).
Can store multiple properties.
Example:
let myVariable = document.querySelector('h1');
Objects can also be:

let person = { name: "Alice", age: 25 };
console.log(person.name); // Output: "Alice"


let iceCream = "chocolate";
if (iceCream === "chocolate") {
  alert("Yay, I love chocolate ice cream!");
} else {
  alert("Awwww, but chocolate is my favorite…");
}
