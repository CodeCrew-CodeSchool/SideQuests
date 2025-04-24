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


```javascript

array literal method: 

let redFruits = ["🍉", "🍒", "🍓", "🍅", "🍎" ]; 

let redFruits = [
 "🍉"
 "🍒",
 "🍓",
 "🍅",
 "🍎"
];

new Array()

let rojoFruit = new Array ("🍉", "🍒", "🍓", "🍅", "🍎" );

document.write(redFruits);
document.write(rojoFruits);

Output:
🍉,🍒,🍓,🍅,🍎
🍉,🍒,🍓,🍅,🍎

```
You can also create an array, and then provide the elements:
```javascript
const Fruits = [];
Fruits[0] = "🍊";
Fruits[1] = "🍑";
Fruits[2] = "🥭";
document.write(Fruits);
Output:
🍊,🍑,🥭
```

### ⭐ Array Properties
- Length: The length property of an array returns the length of an array (the number of array elements).
```javascript
let redFruits = ["🍉", "🍒", "🍓", "🍅", "🍎" ]; 
let length = redFruits.length;
Output:
5
```
### ⭐ Array Properties
- Length: The length property of an array returns the length of an array (the number of array elements).
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
