## ⭐ Reviewing Arrays

It is week 3 day 1 of Module 3 and I decided to review Arrays
- An array is a special variable, which can hold more than one value.
## ⭐ Why Use Arrays
If you have a list of items (a list of fruits, for example), storing the fruits in single variables could look like this: <br>

```javascript

let redFruit1 = "🍉"; 
let redFruit2 = "🍒"; 
let redFruit3 = "🍓"; 
let redFruit4 = "🍅"; 
let redFruit5 = "🍎"; 
console.log(redFruit1,redFruit2,redFruit3,redFruit4,redFruit5);
Output:
🍉🍒🍓🍅🍎
```

However, what if you want to loop through the fruit and find a specific one? And what if you had not 3 fruit, but 20?

⭐✨ The solution is an array! ⭐✨

An array can hold many values under a single name, and you can access the values by referring to an index number.

### ⭐ Creating A Array



## array literal method: 

Array literal notation uses a comma-separated list of values inside square brack
ets to create and initialize an array, like this

```javascript
let redFruits = ["🍉", "🍒", "🍓", "🍅", "🍎" ]; 

let redFruits = [
 "🍉"
 "🍒",
 "🍓",
 "🍅",
 "🍎"
];
```

## Array() constructor

 A constructor function is one that creates and initializes an object. In the case of the 
Array() constructor, it returns a new array object. To use a constructor function, 
use the new operator with the name of the constructor function followed by open 
and close parentheses:

```javascript
new Array()

let rojoFruit = new Array ("🍉", "🍒", "🍓", "🍅", "🍎" );

document.write(redFruits);
document.write(rojoFruits);

Output:
🍉,🍒,🍓,🍅,🍎
🍉,🍒,🍓,🍅,🍎

```
## Arrays by Index

```javascript
const Fruits = [];
Fruits[0] = "🍊";
Fruits[1] = "🍑";
Fruits[2] = "🥭";
document.write(Fruits);
Output:
🍊,🍑,🥭
```
 Using the split function
  The split() function makes an array out of a string. To use split(), give it the 
character (or characters) that you want to use to split the string. For example, if 
you have a text file containing comma-separated values, you can turn it into an 
array by splitting it on the comma:

```javascript 
let fruit = "🍉,🍒,🍓,🍅,🍎"
const fruitArray= fruit.split(',')
```


### ⭐ Array Properties
- Length: The length property of an array returns the length of an array (the number of array elements).
```javascript
let redFruits = ["🍉", "🍒", "🍓", "🍅", "🍎" ]; 
let length = redFruits.length;
Output:
5
```
- Length: The length property of an array returns the length of an array (the number of array elements).
    - For any array, the index of the very last element will always be its length - 1
- push(element1, element2, ...): Adds one or more elements to the end of the array and returns the new length. Think of it like adding to the back of a line.
- pop(): Removes the last element from the array and returns that element. It's like the last person leaving the line. If the array is empty, it returns undefined.
- unshift(element1, element2, ...): Adds one or more elements to the beginning of the array and returns the new length. Imagine adding to the front of the line.
- shift(): Removes the first element from the array and returns that element. It's like the first person leaving the line. If the array is empty, it returns undefined.
- concat(value1, value2, ...): Returns a new array consisting of the calling array joined with other array(s) and/or value(s). The original arrays are not modified.
- forEach() provides a clean and readable way to iterate over array elements and execute a provided function for each one.
```javascript
let redFruits = ["🍉", "🍒", "🍓"]; 
let orangeFruits = ["🍊", "🍑", "🥭"]; 
let fruits = redFruits.concat(orangeFruits);
console.log(fruits);
Output:
["🍉", "🍒", "🍓","🍊", "🍑", "🥭"];
```
- reverse(): Reverses the order of the elements in an array in place. It modifies the original array.
- join(separator): Creates and returns a new string by concatenating all of the elements in an array (or an array-like object), separated by a specified separator string. If no separator is provided, a comma (,) is used.

### Fast Facts about Arrays
-  Arrays keep track of their elements by assigning each element a 
number, called the index.
-  The array’s elements are numbered starting with 0. This is called zero-based 
numbering


## Looping Arrays

```javascript
let fruit = "🍉,🍒,🍓,🍅,🍎";

for (let i = 0; i < fruit.length; i++) {
  console.log(`Character at index ${i}: ${fruit[i]}`);
}
```
```javascript
 const myArray = [3434,56,2];
 let sum = 0;
 for (let i = 0; i<myArray.length-1; i++){
  sum += myArray[i];
 }
 console.log(`The sum is ${sum}`);
output = 3490
 // sum += myArray[i]; is saying sum = sum + myArray[i];
```

## Mapping an Array 
 The map() array function takes a callback function and returns a new array with 
the result of applying the callback function to each element of the array
- the callback don't have to already be defined. 
- The filter() method handles the looping and the conditional checking internally. You provide it with the logic (the callback function) that determines which elements should be kept. This makes your code more concise and easier to read by focusing on what you want to achieve rather than how to achieve it at a low level.

```javascript
const ingredients = [
  'eggs',
  'milk',
  'cheese',
  'garlic',
  'onion',
  'kale',
  'salt',
  'pepper',
 ];
 let listItems = ingredients.map(
  (singleIngredient) => `<li>${singleIngredient}</li>`
 );
```