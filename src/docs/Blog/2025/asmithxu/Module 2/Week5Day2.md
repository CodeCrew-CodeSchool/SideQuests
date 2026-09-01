# Week 5 Day 2 - March 4, 2025
## Traversing the Matrix

Today we practiced manipulating Arrays and using different functions to achieve this. Some of the methods we used included:
 + pop - this removes the last element from the array
 + push - this adds one or more elements to the end of the array and increases its length
 + shift - this removes the first element of the array
 + unshift - this adds one or more elements to the beginning of the array and increases its length

 When you console.log the push and unshift elements, it will give you the resulting length. These are adding elements. When you console.log pop and shift, if will give you the value of the element of the length. 

 The lab involved using these methods and then iterating through an array and sorting out the even and odd numbers. Removing the numbers from the original array was challenging because I tend to use the for statement to iterate up the index. Once you remove the number, the index resets to zero which presents a challenge. I created a solution that involved subtracting i in the iteration expression in the for loop grabbing the length using the index, but that would only work if counting up consecutive numbers. 

 I went over it with Quincy and learned that I could modify i in the actual loop to create my code.