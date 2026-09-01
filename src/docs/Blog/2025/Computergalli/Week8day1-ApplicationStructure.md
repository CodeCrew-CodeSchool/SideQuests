1. getElementsByClassName()
Description:
getElementsByClassName() is a DOM method used to select all elements with a specific class name. This function returns a live HTMLCollection (an array-like object) of all elements that match the class name. You can access individual elements using array indexing.

Example:

const elements = document.getElementsByClassName('my-class'); console.log(elements[0]); // Access the first element with the class 'my-class'
MDN Documentation:
getElementsByClassName() on MDN

2. getAttribute()
Description:
getAttribute() is used to retrieve the value of a specified attribute from an HTML element. This is useful when you need to access custom data attributes such as data-title or data-category.

Example:

const bookTitle = buttonElement.getAttribute('data-title');
MDN Documentation:
getAttribute() on MDN

3. setAttribute()
Description:
setAttribute() allows you to set the value of an attribute on an HTML element. This method is useful when you want to dynamically modify elements or add new attributes.

Example:

element.setAttribute('data-category', 'fiction');
MDN Documentation:
setAttribute() on MDN

4. innerHTML
Description:
innerHTML is a property of DOM elements that gets or sets the HTML content inside the element. This is useful for dynamically changing the contents of a webpage.

Example:

const div = document.getElementsByClassName('content')[0]; div.innerHTML = '<p>New content goes here!</p>';
MDN Documentation:
innerHTML on MDN

5. Event Handling with onclick
Description:
The onclick property is used to assign an event handler function to an HTML element. This allows you to specify what should happen when a user clicks on an element.

Example:

buttonElement.onclick = function() { alert('Button clicked!'); };
MDN Documentation:
onclick on MDN

JavaScript Language Features
1. For-loops
Description:
A for loop is used to repeatedly execute a block of code a set number of times. In the assignment, for-loops are used to iterate through HTMLCollections (from getElementsByClassName) to attach event handlers or manipulate elements.

Syntax:

for (let i = 0; i < collection.length; i++) { // Code to execute on each element }
Example:

const buttons = document.getElementsByClassName('add-to-cart'); for (let i = 0; i < buttons.length; i++) { buttons[i].onclick = function() { // Handle button click }; }
MDN Documentation:
For-loop on MDN

2. Array Indexing with HTMLCollections
Description:
HTMLCollections returned by getElementsByClassName are array-like objects. This means you can access individual elements using an index, just like with arrays.

Example:

const items = document.getElementsByClassName('cart-item'); const firstItem = items[0]; // Access the first item
MDN Documentation:
HTMLCollection on MDN

3. forEach() on NodeLists (Optional Reading)
Though we are not using querySelectorAll() in this assignment, if you were working with NodeList objects, you could use the forEach() method to loop through them. This is not applicable to HTMLCollections.

Example:

const items = document.querySelectorAll('.cart-item'); items.forEach(function(item) { console.log(item.innerHTML); });
MDN Documentation:
forEach() on MDN
