#### Objects are variables too. But objects can contain many values.
#### Object values are written as name : value pairs (name and value separated by a colon)

#### Creating a JavaScript Object
- Create a single object, using an object literal.
```
let person = {firstName:"John", lastName:"Doe", age:50, eyeColor:"blue"};
```
- Create a single object, with the keyword new.
```
const person = new Object();
person.firstName = "John";
person.lastName = "Doe";
```

- Define an object constructor, and then create objects of the constructed type.
```
function Person(first, last, age, eye) {
  this.firstName = first;
  this.lastName = last;
  this.age = age;
  this.eyeColor = eye;
}
const myFather = new Person("John", "Doe", 50, "blue");
const myMother = new Person("Sally", "Rally", 48, "green");
```

- Create an object using Object.create()
```
const person = {
  isHuman: false,
}
const me = Object.create(person);
```
* this key word 
- When used in an object method, this refers to the object.
this refer to person 
```
const person = {
  firstName: "John",
  fullName : function() {
  return this.firstName ;
}
```
- When used alone, this refers to the global object.
```
let x = this; // [object Window]
```
prototype :
all JavaScript objects inherit properties and methods from a prototype.
The Object.prototype is on the top of the prototype inheritance chain:
- Using the prototype Property
 - The JavaScript prototype property allows you to add new properties to object constructors:
 ```
function Person(first, last, age, eyecolor) {
  this.firstName = first;
  this.lastName = last;
  this.age = age;
  this.eyeColor = eyecolor;
}

Person.prototype.nationality = "English";
 ```
- The JavaScript prototype property also allows you to add new methods to objects constructors: 
 ```
function Person(first, last, age, eyecolor) {
  this.firstName = first;
  this.lastName = last;
  this.age = age;
  this.eyeColor = eyecolor;
}

Person.prototype.name = function() {
  return this.firstName + " " + this.lastName;
};
 ```
### Class Syntax :

* Use the keyword class to create a class.
* Always add a method named constructor()
Example :  * creates a class named "Car". * The class has two initial properties: "name" and "year".
 ```
class Car {
  constructor(name, year) {
    this.name = name;
    this.year = year;
  }
}

 ```

* A JavaScript class is not an object.
* It is a template for JavaScript objects
* Using a Class : use the class to create objects:

- Example : 
* creates a class named "Car". The class has two initial properties: "name" and "year".
 ```
const myCar1 = new Car("Ford", 2014);
const myCar2 = new Car("Audi", 2019);
 ```







# link chalenges (https://www.freecodecamp.org/alaa-abuhani)


 
