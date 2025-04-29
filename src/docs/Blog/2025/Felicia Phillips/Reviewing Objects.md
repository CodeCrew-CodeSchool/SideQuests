# ⭐ Objects
Objects are resuable components that contain data and functionality.

In JavaScript, both the data and functionality encapsulated by an object are called **properties**. If a property has a function value, it’s also known as a **method**. 
JavaScript objects can be used to describe physical objects, but they can also be 
used to describe abstract ideas.

example:

```javascript
const pencil = {
  length: "7.5 inches",
  shape: "hexagonal",
  diameter: "1/4 inch",
  write: function(){/*do writing*/},
  erase: function(){/*do erasing*/},
  sharpen: function(){/*do sharpening*/},
 }
 ```

Once object is created, you can find out about it and make use of its functions by using dot notation. 

pencil.sharpen();
 const newPencil = {...pencil}; //makes copies of it

## Javascript has four ways to create objects from scratch

- Use object literal notation.
- Use the new keyword.
- Use Object.create().
- Define a class.


### literal notation

```javascript
const person = {eyes: 2, feet: 2, eyeColor: 'brown'};
```

or

```javascript
 const person = {};
 person.hair = 'black';
 person.hands = 2;
 person.fullName = {firstName:'Lamont',lastName:'Rudnick'};
```


### Object Constructor

A constructor function is very much like a template or a blueprint for creating objects.

- The constructor function itself is the blueprint. It defines the structure and initial properties that objects created from it will have.
- When you call the constructor with new, you are using that blueprint to create a specific instance (the object). Each instance will have the properties and methods defined in the constructor, but with potentially different values for those properties.

function Cat(name, type){
  this.name = name;
  this.type = type;
 }
 const ourCat = new Cat('Murray', 'domestic short hair');

 example:

```javascript
 class Car {
  constructor(make, model, year) {
    this.make = make;
    this.model = model;
    this.year = year;
  }

  getDescription() {
    return `${this.year} ${this.make} ${this.model}`;
  }
}

const car1 = new Car("Toyota", "Camry", 2023);
const car2 = new Car("Honda", "Civic", 2022);

console.log(car1.make);          // Output: Toyota
console.log(car2.getDescription()); // Output: 2022 Honda Civic
```


###  Making objects with class


 class Pet {
  constructor(name,type){
    this.name = name;
    this.type = type;
  }
 }
 const ourDog = new Pet('Chauncey','AmStaff');

 