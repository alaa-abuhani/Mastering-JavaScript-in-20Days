* javascript have primitive data type are immutable

-string

-number

-boolean

-null 

-undefine


* javascript have object data type and array is special kind of object

* object and array mutable
 * An array is a special variable, which can hold more than one value:

example :
```
const cars = ["Saab", "Volvo", "BMW"];
```
* Looping Array Elements : use the Array.forEach() function
* example : 
```
const fruits = ["Banana", "Orange", "Apple", "Mango"];

let text = "<ul>";
fruits.forEach(myFunction);
text += "</ul>";

function myFunction(value) {
  text += "<li>" + value + "</li>";
}
```
* Adding Array Elements : the easiest way to add a new element to an array is using the push() method
example :
```
const fruits = ["Banana", "Orange", "Apple"];
fruits.push("Lemon");  // Adds a new element (Lemon) to fruits
```
* JavaScript Array pop() : The pop() method removes the last element from an array
* The pop() method returns the value that was "popped out" 
```
const fruits = ["Banana", "Orange", "Apple", "Mango"];
let fruit = fruits.pop();
```
JavaScript Array push() : The push() method adds a new element to an array (at the end)
```
const fruits = ["Banana", "Orange", "Apple", "Mango"];
fruits.push("Kiwi");
```
* The push() method returns the new array length:
```
const fruits = ["Banana", "Orange", "Apple", "Mango"];
let length = fruits.push("Kiwi"); // 5
```
* Shifting Elements : The shift() method removes the first array element and "shifts" all other elements to a lower index. & he shift() method returns the value that was "shifted out":

```
const fruits = ["Banana", "Orange", "Apple", "Mango"];
let fruit = fruits.shift();
```
* JavaScript Array unshift() :The unshift() method adds a new element to an array (at the beginning), and "unshifts" older elements &
The unshift() method returns the new array length:
example :
```
const fruits = ["Banana", "Orange", "Apple", "Mango"];
fruits.unshift("Lemon");
```




* immutable variables can assign to mutable value



1 # basic-data-structures/copy-array-items-using-slice
```
function forecast(arr) {
  // Only change code below this line
arr=arr.slice(2,4)
  return arr;
}

// Only change code above this line
console.log(forecast(['cold', 'rainy', 'warm', 'sunny', 'cool', 'thunderstorms']));
```
2 # copy-an-array-with-the-spread-operator
```
function copyMachine(arr, num) {
  let newArr = [];
  while (num >= 1) {
    // Only change code below this line
newArr.push([...arr])
    // Only change code above this line
    num--;
  }
  return newArr;
}


console.log(copyMachine([true, false, true], 2));
```

3 # profile-lookup
```
// Setup
const contacts = [
  {
    firstName: "Akira",
    lastName: "Laine",
    number: "0543236543",
    likes: ["Pizza", "Coding", "Brownie Points"],
  },
  {
    firstName: "Harry",
    lastName: "Potter",
    number: "0994372684",
    likes: ["Hogwarts", "Magic", "Hagrid"],
  },
  {
    firstName: "Sherlock",
    lastName: "Holmes",
    number: "0487345643",
    likes: ["Intriguing Cases", "Violin"],
  },
  {
    firstName: "Kristian",
    lastName: "Vos",
    number: "unknown",
    likes: ["JavaScript", "Gaming", "Foxes"],
  },
];

function lookUpProfile(name, prop) {
  // Only change code below this line
for (var x =0 ; x<contacts.length ;x++){
  if (contacts[x].firstName == name){
    
  if (contacts[x].likes == prop)
  return prop
  
  if(prop=="likes")
    return contacts[x].likes
  
  if(prop=="lastName")
    return contacts[x].lastName
 
  return "No such property"
  }  
}
return "No such contact"


  // Only change code above this line
}

lookUpProfile("Akira", "likes");
```
4 # write-reusable-javascript-with-functions
```
function reusableFunction(){
  console.log("Hi World");
}
reusableFunction()
```
5 # understanding-undefined-value-returned-from-a-function

```
// Setup
let sum = 0;

function addThree() {
  sum = sum + 3;
}

// Only change code below this line
function addFive() {
  sum = sum + 5;
}

// Only change code above this line

addThree();
addFive();
```
6 # return-a-value-from-a-function-with-return
```
function timesFive(num) {
  return num * 5;
}

const answer = timesFive(5);
```

