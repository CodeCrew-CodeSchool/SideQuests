## ⭐ Reviewing Loops

It is week 2 day 3 of Module 3 and I decided to review loops.

- Loops in JavaScript are control flow statements that allow for the repeated execution of a block of code.
- They allow for concise and efficient execution of repetitive tasks, making them essential for various programming scenarios. 

## ⭐ for Loops
- The for loop is commonly used when the number of iterations is known beforehand. 
- Initialization: Executed once before the loop starts.
- Condition: Evaluated before each iteration; the loop continues as long as the condition is true.
- Increment/Decrement: Executed after each iteration.

### ⭐ Example:
```javascript
for (Initialization; Condition; Increment/Decrement) {
  Action or Task that will be repeated
};
```


```javascript
for (let i = 0; i < 5; i++) {
  console.log(i);
} 
Output: 0 1 2 3 4
```

## ⭐ while Loops
- In JavaScript, a while loop repeatedly executes a block of code as long as a specified condition remains true. 
- Initialization: Sets up the necessary variables before the loop starts.
- Condition: Modifies the variables involved in the condition, usually to ensure the loop eventually terminates.

### ⭐ Example:
```javascript
Initialization; 
while (condition)  {
  Task 
  Increment/Decrement
}
```

```javascript
let i = 1;
while (i <= 5)  {
  console.log(i);
  i++;
}
```

## ⭐ When to use for or while loops

Use for <code>Loops</code> When:

You know the number of iterations in advance (or it's easily determined): for loops are excellent when you need to iterate a specific number of times. This is common when working with arrays, strings, or any seque

Use <code>while</code> Loops When:

The number of iterations is unknown or depends on a condition that might change during the loop's execution: while loops are ideal when you need to continue looping as long as a certain condition remains true, and you don't know beforehand how many times that will be.

## ⭐ Practice

Create a loop for this: 

<code>
fill(17, 0, 255);
var x = 0; <br>
text(x, x, 10); <br>
text(x+50, x+50, 10); <br>
text(x+100, x+100, 10); <br>
text(x+150, x+150, 10); <br>
text(x+200, x+200, 10); <br>
text(x+250, x+250, 10); <br>
text(x+300, x+300, 10); <br>
text(x+350, x+350, 10); <br>
</code>
<br>

1) What do you want to repeat each time? text()
2) What value do you want to change each time?  horizontal and vertical position
3) When do you want to stop looping? stop the loop when we've drawn the text elements up to the position x = 350

<br>
<code>
let x = 0; // Initialize <br>
while (x <= 350) // Condition <br> { 
  text(x, x, 10); <br>
  x += 50; // Increment
}
</code>


### Projects I have developed this week:
1. [Scoops](https://cloverdeveloped.github.io/scoops/)
2. [Portfolio Template](https://cloverdeveloped.github.io/cloverdev/)

### ⭐Outside of class:
After class, I freelance as a graphic designer for B Visible. I'm currently designing a magazine. 

