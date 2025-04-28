## ⭐ Basic Javascript


### Funcation declaration 

A function declaration is a function that is bound to an identifier, or name. 

function declaration example:

```javascript
function identifier() {
 //statements or instructions that are executed by the browser
}
```

Calling function 

```javascript 
identifier();
```

This function call executes the function body, or all of the statements between the curly braces in the function declaration.



### Default Parameters 

 Default parameters allow parameters to have a predetermined value in case there is no argument passed into the function or if the argument is undefined when called.


```javascript
 function greeting (name = 'stranger') {
  console.log(`Hello, ${name}!`)
}

greeting('Nick') // Output: Hello, Nick!
greeting() // Output: Hello, stranger!
```

To pass back information from the function call, we use a return statement.