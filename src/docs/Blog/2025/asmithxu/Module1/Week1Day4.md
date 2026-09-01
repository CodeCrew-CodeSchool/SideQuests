# Week 1 Day 4 - February 6, 2025
## Creating Forms

Today we learned how to create forms using HTML. We learned about the different elements that would be used to create a form along with their attributes. Some of these elements include:
 - Form
 - Input
 - Label
 - Button
 - Text area

We had a project today that involved creating a form that would send information to our email address. I was able to create the form - you can check it out <a href="https://asmithxu.github.io/ContactMeForm/">here</a>.

When I was creating the form, I played around a little with some of the settings. It was interesting to me that there are a couple of ways to include a button - you can use the button element or you can include the type="submit" attribute in the input element. 

In the end, I decided to got with the second one because I found that I was not getting the information sent over email with just the button element. 

Also, I tried different values for the enctype attribute and found that text/plain gave me what I wanted. However, I got multiple security warnings when I used it after deploying my website. 

The class was interested in form validity - having an input that has specific requirements, like a password field that requires you to have a special character. We learned that this was a Javascript only property so we probably would not be able to do that until later in the course.