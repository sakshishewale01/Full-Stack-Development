Absolutely. Since you already have the **Day 1 fundamentals**, for **Day 2** we should not just memorize syntax. We’ll build a proper understanding of the concepts because these are the JavaScript features you will use constantly when you start building real projects with **React, Node.js, and Express.js**.

# JavaScript Day 2 — Arrays, Objects, Functions & Modern JavaScript

## 🎯 Day 2 Learning Path

We will learn in this order:

```text
DAY 2

1. Arrays
   ↓
2. Array indexing
   ↓
3. Adding / removing elements
   ↓
4. Looping through arrays
   ↓
5. Objects
   ↓
6. Accessing object data
   ↓
7. Modifying objects
   ↓
8. Nested objects
   ↓
9. Functions
   ↓
10. Parameters & Arguments
   ↓
11. return
   ↓
12. Function scope
   ↓
13. Arrow Functions
   ↓
14. Array Methods
       map()
       filter()
       find()
       forEach()
       reduce()
       some()
       every()
   ↓
15. Destructuring
   ↓
16. Spread Operator
   ↓
17. Rest Operator
   ↓
18. Modern JavaScript syntax
```

---

# 1. ARRAYS

## What is an Array?

An array is a data structure used to store **multiple values inside a single variable**.

Suppose we want to store five student names.

Without an array:

```javascript
let student1 = "Sakshi";
let student2 = "Amit";
let student3 = "Rahul";
let student4 = "Priya";
let student5 = "Neha";
```

This becomes difficult to manage.

Instead:

```javascript
let students = [
    "Sakshi",
    "Amit",
    "Rahul",
    "Priya",
    "Neha"
];
```

Now all five names are stored inside one variable:

```text
students
    ↓
["Sakshi", "Amit", "Rahul", "Priya", "Neha"]
```

This is an array.

---

# 2. Creating an Array

The most common syntax is:

```javascript
let fruits = ["Apple", "Banana", "Mango"];
```

You can also create an empty array:

```javascript
let students = [];
```

Then add elements later.

---

# 3. Arrays Can Store Different Data Types

JavaScript arrays can contain different types of values.

```javascript
let data = [
    "Sakshi",
    20,
    true,
    null
];
```

However, in real applications, arrays are usually used to store related data.

For example:

```javascript
let marks = [85, 90, 78, 92];
```

or:

```javascript
let names = ["Sakshi", "Amit", "Rahul"];
```

---

# 4. Array Index

This is extremely important.

JavaScript arrays use **zero-based indexing**.

That means the first element is at index `0`.

Example:

```javascript
let fruits = [
    "Apple",
    "Banana",
    "Mango",
    "Orange"
];
```

Their indexes are:

```text
Index       Value

  0         Apple
  1         Banana
  2         Mango
  3         Orange
```

So:

```javascript
console.log(fruits[0]);
```

Output:

```text
Apple
```

And:

```javascript
console.log(fruits[2]);
```

Output:

```text
Mango
```

---

# 5. Why Does Array Index Start from 0?

Think of the index as the **distance from the beginning**.

The first element is at distance `0`.

```text
Array:

Apple    Banana    Mango
  ↑
index 0
```

Therefore:

```text
first element  → 0
second element → 1
third element  → 2
```

This is common in programming languages.

---

# 6. Changing an Array Element

Arrays are mutable.

That means we can change their contents.

```javascript
let fruits = ["Apple", "Banana", "Mango"];

fruits[1] = "Orange";

console.log(fruits);
```

Output:

```text
["Apple", "Orange", "Mango"]
```

We changed:

```text
Banana → Orange
```

---

# 7. Array length

Use:

```javascript
array.length
```

Example:

```javascript
let fruits = ["Apple", "Banana", "Mango"];

console.log(fruits.length);
```

Output:

```text
3
```

`length` tells us how many elements are currently in the array.

---

# 8. Adding Elements — push()

`push()` adds an element to the **end** of an array.

```javascript
let fruits = ["Apple", "Banana"];

fruits.push("Mango");

console.log(fruits);
```

Output:

```text
["Apple", "Banana", "Mango"]
```

You can add multiple elements:

```javascript
fruits.push("Orange", "Grapes");
```

---

# 9. Removing Elements — pop()

`pop()` removes the **last element**.

```javascript
let fruits = ["Apple", "Banana", "Mango"];

fruits.pop();

console.log(fruits);
```

Output:

```text
["Apple", "Banana"]
```

---

# 10. Adding at the Beginning — unshift()

`unshift()` adds an element to the beginning.

```javascript
let fruits = ["Banana", "Mango"];

fruits.unshift("Apple");

console.log(fruits);
```

Output:

```text
["Apple", "Banana", "Mango"]
```

---

# 11. Removing from the Beginning — shift()

`shift()` removes the first element.

```javascript
let fruits = ["Apple", "Banana", "Mango"];

fruits.shift();

console.log(fruits);
```

Output:

```text
["Banana", "Mango"]
```

---

# 12. Array Methods — Basic Summary

Remember these four first:

| Method      | Purpose               |
| ----------- | --------------------- |
| `push()`    | Add at end            |
| `pop()`     | Remove from end       |
| `unshift()` | Add at beginning      |
| `shift()`   | Remove from beginning |

Think:

```text
push()      → Add → End
pop()       → Remove → End

unshift()   → Add → Beginning
shift()     → Remove → Beginning
```

---

# 13. Looping Through an Array

Suppose:

```javascript
let students = [
    "Sakshi",
    "Amit",
    "Rahul",
    "Priya"
];
```

We can use a normal `for` loop:

```javascript
for (let i = 0; i < students.length; i++) {

    console.log(students[i]);

}
```

Output:

```text
Sakshi
Amit
Rahul
Priya
```

Notice:

```javascript
students[i]
```

means:

> Give me the element at the current index.

---

# 14. for...of Loop

JavaScript also provides a simpler way to loop through values.

```javascript
let students = ["Sakshi", "Amit", "Rahul"];

for (let student of students) {

    console.log(student);

}
```

Output:

```text
Sakshi
Amit
Rahul
```

This is very useful when you simply want each value.

---

# 15. Important Difference

Normal `for` loop:

```javascript
for (let i = 0; i < students.length; i++) {
    console.log(students[i]);
}
```

You get the **index**:

```text
0
1
2
```

`for...of`:

```javascript
for (let student of students) {
    console.log(student);
}
```

You directly get the **value**.

---

# 16. OBJECTS

Now we come to one of the most important JavaScript concepts.

## What is an Object?

An object stores information in **key-value pairs**.

Example:

```javascript
let student = {

    name: "Sakshi",
    age: 20,
    branch: "Computer Engineering",
    cgpa: 8.9

};
```

Think of it like:

```text
student
   |
   ├── name   → Sakshi
   ├── age    → 20
   ├── branch → Computer Engineering
   └── cgpa   → 8.9
```

---

# 17. Why Do We Need Objects?

Suppose we have:

```javascript
let studentName = "Sakshi";
let studentAge = 20;
let studentBranch = "Computer Engineering";
let studentCGPA = 8.9;
```

These variables belong to the same student, but they are separate.

An object groups related information together:

```javascript
let student = {

    name: "Sakshi",
    age: 20,
    branch: "Computer Engineering",
    cgpa: 8.9

};
```

This is much easier to manage.

---

# 18. Object Properties

Inside an object:

```javascript
name: "Sakshi"
```

is called a property.

Here:

```text
name  → key
Sakshi → value
```

Another example:

```javascript
age: 20
```

Here:

```text
age → key
20  → value
```

---

# 19. Accessing Object Properties

There are two main ways.

## Dot notation

```javascript
console.log(student.name);
```

Output:

```text
Sakshi
```

Another:

```javascript
console.log(student.age);
```

Output:

```text
20
```

---

# 20. Bracket Notation

We can also use:

```javascript
console.log(student["name"]);
```

Output:

```text
Sakshi
```

Both are valid.

---

# 21. Dot vs Bracket Notation

Usually use:

```javascript
student.name
```

when you know the property name.

Bracket notation becomes especially useful when the property name is stored in a variable.

Example:

```javascript
let property = "name";

console.log(student[property]);
```

Output:

```text
Sakshi
```

---

# 22. Modifying an Object

Objects are mutable.

We can change a property:

```javascript
student.age = 21;
```

Now:

```javascript
console.log(student.age);
```

Output:

```text
21
```

---

# 23. Adding a New Property

We can add a property:

```javascript
student.city = "Pune";
```

Now the object contains:

```javascript
{
    name: "Sakshi",
    age: 21,
    branch: "Computer Engineering",
    cgpa: 8.9,
    city: "Pune"
}
```

---

# 24. Deleting a Property

Use `delete`.

```javascript
delete student.city;
```

Now `city` is removed.

---

# 25. Object with Different Data Types

An object can contain different data types.

```javascript
let student = {

    name: "Sakshi",
    age: 20,
    isStudent: true,
    cgpa: 8.9,
    skills: ["Java", "JavaScript", "HTML"]

};
```

Notice that an object can even contain an array.

This is extremely common in real applications.

---

# 26. Nested Objects

An object can contain another object.

```javascript
let student = {

    name: "Sakshi",

    address: {

        city: "Pune",
        state: "Maharashtra"

    }

};
```

Access:

```javascript
console.log(student.address.city);
```

Output:

```text
Pune
```

---

# 27. Array of Objects

This is **extremely important for full-stack development**.

Suppose we have multiple students.

```javascript
let students = [

    {
        name: "Sakshi",
        age: 20
    },

    {
        name: "Amit",
        age: 21
    },

    {
        name: "Rahul",
        age: 20
    }

];
```

Now:

```javascript
console.log(students[0].name);
```

Output:

```text
Sakshi
```

Why?

```text
students
   ↓
array
   ↓
students[0]
   ↓
object
   ↓
.name
   ↓
"Sakshi"
```

You will see this structure constantly when working with APIs and React.

---

# 28. FUNCTIONS

Now we move to one of the most important concepts in programming.

## What is a Function?

A function is a reusable block of code designed to perform a particular task.

Instead of writing the same code repeatedly:

```javascript
console.log("Hello");
console.log("Hello");
console.log("Hello");
```

we can create:

```javascript
function greet() {

    console.log("Hello");

}
```

Then call it:

```javascript
greet();
```

---

# 29. Function Syntax

```javascript
function functionName() {

    // code

}
```

Example:

```javascript
function greet() {

    console.log("Hello");

}
```

Calling the function:

```javascript
greet();
```

---

# 30. Why Functions Are Important

Functions provide:

### Reusability

Write once and use multiple times.

### Organization

Break large programs into smaller pieces.

### Maintainability

Changing one function can update the behavior everywhere it is used.

### Abstraction

You don't need to know the internal implementation to use a function.

---

# 31. Function Parameters

A parameter allows a function to receive information.

```javascript
function greet(name) {

    console.log(`Hello ${name}`);

}
```

Now:

```javascript
greet("Sakshi");
```

Output:

```text
Hello Sakshi
```

Here:

```text
name → parameter
"Sakshi" → argument
```

---

# 32. Parameter vs Argument

This is an important distinction.

Function definition:

```javascript
function greet(name) {

}
```

`name` is the **parameter**.

Function call:

```javascript
greet("Sakshi");
```

`"Sakshi"` is the **argument**.

Remember:

```text
Parameter → placeholder
Argument  → actual value
```

---

# 33. Multiple Parameters

A function can accept multiple parameters.

```javascript
function add(a, b) {

    console.log(a + b);

}
```

Call:

```javascript
add(10, 20);
```

Output:

```text
30
```

Here:

```text
a = 10
b = 20
```

---

# 34. return

A function can return a value.

Example:

```javascript
function add(a, b) {

    return a + b;

}
```

Now:

```javascript
let result = add(10, 20);

console.log(result);
```

Output:

```text
30
```

---

# 35. console.log vs return

This is very important.

### console.log()

Displays something.

```javascript
function add(a, b) {

    console.log(a + b);

}
```

### return

Sends the value back to the place where the function was called.

```javascript
function add(a, b) {

    return a + b;

}
```

Then:

```javascript
let result = add(10, 20);
```

Now `result` contains:

```text
30
```

### Remember

```text
console.log() → show value
return        → give value back
```

---

# 36. Function Without Parameters

```javascript
function sayHello() {

    return "Hello";

}

let message = sayHello();

console.log(message);
```

---

# 37. Function with Parameters and Return

This is the most common pattern.

```javascript
function calculateTotal(price, quantity) {

    return price * quantity;

}

let total = calculateTotal(100, 3);

console.log(total);
```

Output:

```text
300
```

---

# 38. Default Parameters

We can provide a default value.

```javascript
function greet(name = "User") {

    console.log(`Hello ${name}`);

}
```

If we call:

```javascript
greet();
```

Output:

```text
Hello User
```

If we call:

```javascript
greet("Sakshi");
```

Output:

```text
Hello Sakshi
```

---

# 39. Function Scope

Variables declared inside a function are normally accessible only inside that function.

```javascript
function test() {

    let message = "Hello";

    console.log(message);

}

test();
```

This works.

But:

```javascript
console.log(message);
```

outside the function will not work.

---

# 40. Arrow Functions

Modern JavaScript introduced arrow functions.

Normal function:

```javascript
function add(a, b) {

    return a + b;

}
```

Arrow function:

```javascript
const add = (a, b) => {

    return a + b;

};
```

Same basic purpose, different syntax.

---

# 41. Arrow Function — Short Form

If there is only one expression:

```javascript
const add = (a, b) => a + b;
```

This automatically returns:

```text
a + b
```

So:

```javascript
const result = add(10, 20);

console.log(result);
```

Output:

```text
30
```

---

# 42. Arrow Function with One Parameter

You can write:

```javascript
const square = number => number * number;
```

instead of:

```javascript
const square = (number) => number * number;
```

Both are valid.

---

# 43. When Should You Use Arrow Functions?

You will use arrow functions heavily in:

```text
Array methods
React
Event handlers
Callbacks
Promises
Modern JavaScript
```

Example:

```javascript
students.map(student => student.name);
```

This syntax will become very important.

---

# 44. CALLBACK FUNCTIONS

A callback is a function passed into another function.

Example:

```javascript
function greet(name) {

    console.log(`Hello ${name}`);

}

function processUser(callback) {

    callback("Sakshi");

}

processUser(greet);
```

Here:

```text
greet
   ↓
passed as a function
   ↓
processUser()
```

You will see callbacks frequently with array methods and asynchronous JavaScript.

---

# 45. ARRAY METHODS

Now we reach one of the **most important parts of Day 2**.

Instead of manually writing loops for everything, JavaScript provides array methods.

The important ones for you are:

```text
forEach()
map()
filter()
find()
some()
every()
reduce()
```

These are extremely important for:

```text
Frontend development
React
APIs
Data processing
Backend development
```

---

# 46. forEach()

`forEach()` executes a function for every element.

Example:

```javascript
let numbers = [10, 20, 30];

numbers.forEach(function(number) {

    console.log(number);

});
```

Output:

```text
10
20
30
```

Modern syntax:

```javascript
numbers.forEach(number => {

    console.log(number);

});
```

---

# 47. forEach() with Index

You can also get the index.

```javascript
let students = ["Sakshi", "Amit", "Rahul"];

students.forEach((student, index) => {

    console.log(index, student);

});
```

Output:

```text
0 Sakshi
1 Amit
2 Rahul
```

---

# 48. map()

`map()` creates a **new array** by transforming every element.

Example:

```javascript
let numbers = [1, 2, 3, 4];

let doubled = numbers.map(number => number * 2);

console.log(doubled);
```

Output:

```text
[2, 4, 6, 8]
```

Original array:

```text
[1, 2, 3, 4]
```

New array:

```text
[2, 4, 6, 8]
```

---

# 49. map() — Important Concept

Think:

```text
Original
   ↓
[1, 2, 3, 4]

map()
   ↓
Transform each element

Result
   ↓
[2, 4, 6, 8]
```

Use `map()` when you want to **transform data**.

---

# 50. filter()

`filter()` creates a new array containing only elements that satisfy a condition.

Example:

```javascript
let numbers = [10, 15, 20, 25, 30];

let evenNumbers = numbers.filter(number => number % 2 === 0);

console.log(evenNumbers);
```

Output:

```text
[10, 20, 30]
```

Think:

```text
Original
[10, 15, 20, 25, 30]

filter()
     ↓
Keep only even numbers

[10, 20, 30]
```

---

# 51. find()

`find()` returns the **first element** that satisfies a condition.

```javascript
let numbers = [10, 20, 30, 40];

let result = numbers.find(number => number > 25);

console.log(result);
```

Output:

```text
30
```

It stops after finding the first matching element.

---

# 52. find() with Objects

This is very useful in real applications.

```javascript
let users = [

    { id: 1, name: "Sakshi" },

    { id: 2, name: "Amit" },

    { id: 3, name: "Rahul" }

];

let user = users.find(user => user.id === 2);

console.log(user);
```

Output:

```javascript
{
    id: 2,
    name: "Amit"
}
```

---

# 53. some()

`some()` checks whether **at least one element** satisfies a condition.

```javascript
let numbers = [1, 3, 5, 8];

let result = numbers.some(number => number % 2 === 0);

console.log(result);
```

Output:

```text
true
```

Because `8` is even.

Think:

```text
some()
↓
"Does at least ONE satisfy the condition?"
```

---

# 54. every()

`every()` checks whether **all elements** satisfy a condition.

```javascript
let numbers = [2, 4, 6, 8];

let result = numbers.every(number => number % 2 === 0);

console.log(result);
```

Output:

```text
true
```

Think:

```text
every()
↓
"Do ALL elements satisfy the condition?"
```

---

# 55. some() vs every()

Very important:

```text
some()
→ At least one

every()
→ All
```

Example:

```javascript
[2, 4, 5].some(x => x % 2 === 0);
```

Result:

```text
true
```

because `2` and `4` are even.

But:

```javascript
[2, 4, 5].every(x => x % 2 === 0);
```

Result:

```text
false
```

because `5` is not even.

---

# 56. reduce()

`reduce()` is used to combine all array elements into a single result.

Example:

```javascript
let numbers = [10, 20, 30, 40];

let total = numbers.reduce(
    (sum, number) => sum + number,
    0
);

console.log(total);
```

Output:

```text
100
```

Think:

```text
10
 ↓
10 + 20 = 30
 ↓
30 + 30 = 60
 ↓
60 + 40 = 100
```

Final result:

```text
100
```

---

# 57. reduce() Components

```javascript
numbers.reduce(
    (sum, number) => sum + number,
    0
);
```

Here:

```text
sum
    → accumulated result

number
    → current element

0
    → initial value
```

---

# 58. Array Methods Summary

| Method      | Purpose                       | Returns               |
| ----------- | ----------------------------- | --------------------- |
| `forEach()` | Execute code for each element | Usually `undefined`   |
| `map()`     | Transform elements            | New array             |
| `filter()`  | Select elements               | New array             |
| `find()`    | Find first matching element   | Element / `undefined` |
| `some()`    | Check if at least one matches | Boolean               |
| `every()`   | Check if all match            | Boolean               |
| `reduce()`  | Combine values                | Single result         |

---

# 59. map() vs forEach()

Very important interview question.

### forEach()

```javascript
numbers.forEach(number => {

    console.log(number);

});
```

Main purpose:

> Perform an action for each element.

### map()

```javascript
let doubled = numbers.map(number => number * 2);
```

Main purpose:

> Transform each element and create a new array.

Remember:

```text
forEach → do something
map     → transform something
```

---

# 60. Chaining Array Methods

Array methods can be combined.

Example:

```javascript
let numbers = [1, 2, 3, 4, 5, 6];

let result = numbers
    .filter(number => number % 2 === 0)
    .map(number => number * 2);

console.log(result);
```

First:

```text
[1,2,3,4,5,6]
       ↓
filter even
       ↓
[2,4,6]
       ↓
map × 2
       ↓
[4,8,12]
```

This style is extremely common in modern JavaScript and React.

---

# 61. DESTRUCTURING

Destructuring allows us to extract values from arrays or objects easily.

## Array Destructuring

```javascript
let colors = ["Red", "Green", "Blue"];

let [first, second, third] = colors;

console.log(first);
console.log(second);
console.log(third);
```

Output:

```text
Red
Green
Blue
```

---

# 62. Object Destructuring

Suppose:

```javascript
let student = {

    name: "Sakshi",
    age: 20,
    city: "Pune"

};
```

Without destructuring:

```javascript
console.log(student.name);
console.log(student.age);
```

With destructuring:

```javascript
let { name, age } = student;

console.log(name);
console.log(age);
```

Much cleaner.

---

# 63. Why Destructuring Matters

You will use destructuring heavily in React.

For example:

```javascript
const { name, age } = student;
```

Instead of repeatedly writing:

```javascript
student.name
student.age
```

---

# 64. Spread Operator (...)

The spread operator is:

```text
...
```

It expands elements from an iterable such as an array.

Example:

```javascript
let numbers1 = [1, 2, 3];

let numbers2 = [...numbers1, 4, 5];

console.log(numbers2);
```

Output:

```text
[1, 2, 3, 4, 5]
```

---

# 65. Copying an Array

```javascript
let original = [1, 2, 3];

let copy = [...original];
```

Now:

```text
original → [1,2,3]
copy     → [1,2,3]
```

This creates a new array.

This becomes very important in React state management.

---

# 66. Combining Arrays

```javascript
let frontend = ["HTML", "CSS"];

let programming = ["JavaScript", "Java"];

let skills = [...frontend, ...programming];

console.log(skills);
```

Output:

```text
["HTML", "CSS", "JavaScript", "Java"]
```

---

# 67. Spread with Objects

Spread also works with objects.

```javascript
let student = {

    name: "Sakshi",
    age: 20

};

let updatedStudent = {

    ...student,
    city: "Pune"

};
```

Result:

```javascript
{
    name: "Sakshi",
    age: 20,
    city: "Pune"
}
```

---

# 68. Updating an Object Using Spread

Suppose:

```javascript
let student = {

    name: "Sakshi",
    age: 20

};
```

We want to change age:

```javascript
let updatedStudent = {

    ...student,
    age: 21

};
```

This creates a new object.

This pattern is extremely important in React.

---

# 69. REST OPERATOR

The rest operator also uses:

```text
...
```

But its purpose is different.

It collects multiple values into one array.

Example:

```javascript
function add(...numbers) {

    console.log(numbers);

}

add(10, 20, 30, 40);
```

Output:

```text
[10, 20, 30, 40]
```

Here `...numbers` collects all arguments.

---

# 70. Spread vs Rest

Same syntax:

```text
...
```

Different purpose.

### Spread

Expands values:

```javascript
let arr2 = [...arr1];
```

Think:

```text
ONE → MANY
```

### Rest

Collects values:

```javascript
function test(...values) {}
```

Think:

```text
MANY → ONE
```

This distinction is important.

---

# 71. Modern JavaScript — const by Default

Modern JavaScript style generally follows:

```javascript
const name = "Sakshi";
```

Use `let` only when reassignment is required:

```javascript
let count = 0;

count++;
```

Avoid unnecessary `var`.

---

# 72. Optional Chaining

This is another useful modern feature.

Suppose:

```javascript
let user = {

    name: "Sakshi"

};
```

We want:

```javascript
console.log(user.address.city);
```

This can cause an error because `address` does not exist.

Instead:

```javascript
console.log(user.address?.city);
```

The `?.` operator safely checks whether the previous value exists.

Result:

```text
undefined
```

This is very useful when working with API data.

---

# 73. Nullish Coalescing Operator

The operator:

```text
??
```

provides a fallback when a value is `null` or `undefined`.

Example:

```javascript
let username = null;

let name = username ?? "Guest";

console.log(name);
```

Output:

```text
Guest
```

---

# 74. Practical Example — Student Data

Now let's combine multiple Day 2 concepts.

```javascript
const students = [

    {
        name: "Sakshi",
        marks: 90
    },

    {
        name: "Amit",
        marks: 75
    },

    {
        name: "Rahul",
        marks: 85
    }

];
```

Find students who scored more than 80:

```javascript
const topStudents = students.filter(
    student => student.marks > 80
);

console.log(topStudents);
```

Result:

```text
Sakshi
Rahul
```

---

# 75. Practical Example — Extract Names

```javascript
const students = [

    {
        name: "Sakshi",
        marks: 90
    },

    {
        name: "Amit",
        marks: 75
    },

    {
        name: "Rahul",
        marks: 85
    }

];

const names = students.map(student => student.name);

console.log(names);
```

Output:

```text
["Sakshi", "Amit", "Rahul"]
```

---

# 76. Practical Example — Find a User

```javascript
const users = [

    {
        id: 1,
        name: "Sakshi"
    },

    {
        id: 2,
        name: "Amit"
    },

    {
        id: 3,
        name: "Rahul"
    }

];

const user = users.find(user => user.id === 2);

console.log(user);
```

Output:

```text
{
    id: 2,
    name: "Amit"
}
```

This is similar to how you will process API responses.

---

# 77. Practical Example — Calculate Total

```javascript
const prices = [100, 200, 300];

const total = prices.reduce(
    (sum, price) => sum + price,
    0
);

console.log(total);
```

Output:

```text
600
```

---

# 78. Practical Example — Cart

This is closer to a real application.

```javascript
const cart = [

    {
        name: "Laptop",
        price: 50000,
        quantity: 1
    },

    {
        name: "Mouse",
        price: 1000,
        quantity: 2
    },

    {
        name: "Keyboard",
        price: 2000,
        quantity: 1
    }

];
```

Calculate total:

```javascript
const total = cart.reduce(
    (sum, item) =>
        sum + item.price * item.quantity,
    0
);

console.log(total);
```

This is the type of logic you will encounter in actual applications.

---

# 79. The Most Important Day 2 Concepts for Software Development

You don't need to treat every concept equally.

Focus strongly on:

### ⭐⭐⭐ Very Important

```text
Arrays
Objects
Functions
Arrow Functions
map()
filter()
find()
forEach()
reduce()
Destructuring
Spread Operator
```

### ⭐⭐ Important

```text
some()
every()
Rest Operator
Default Parameters
Optional Chaining
Nullish Coalescing
```

---

# 80. How Day 2 Connects to React

You will soon see code like:

```javascript
const users = data.map(user => (

    <div>
        {user.name}
    </div>

));
```

This uses:

```text
Array
↓
map()
↓
Arrow Function
↓
Object
↓
Object property
```

Another common React pattern:

```javascript
const updatedUser = {

    ...user,

    name: "New Name"

};
```

This uses:

```text
Object
+
Spread Operator
```

So Day 2 is **very important before React**.

---

# 81. Day 2 Mental Model

Try to remember the concepts this way:

```text
ARRAY
↓
Store multiple values

OBJECT
↓
Store related information

FUNCTION
↓
Reuse logic

ARROW FUNCTION
↓
Short modern function syntax

forEach()
↓
Do something for every item

map()
↓
Transform every item

filter()
↓
Select some items

find()
↓
Find one item

some()
↓
Does at least one match?

every()
↓
Do all match?

reduce()
↓
Combine into one result

DESTRUCTURING
↓
Extract values easily

SPREAD
↓
Expand / copy

REST
↓
Collect multiple values
```

---

# 82. Day 2 Practice Problems

Don't just read these concepts. Write these programs yourself.

### Beginner

1. Create an array of 5 fruits.
2. Print the first and last element.
3. Add an element using `push()`.
4. Remove an element using `pop()`.
5. Find the length of an array.
6. Print all elements using a `for` loop.
7. Print all elements using `for...of`.

### Objects

8. Create a student object.
9. Print the student's name.
10. Change the student's age.
11. Add a new property.
12. Delete a property.
13. Create an object containing an address object.
14. Create an array of student objects.

### Functions

15. Create a function to add two numbers.
16. Create a function to calculate the square of a number.
17. Create a function to check even/odd.
18. Create a function to calculate factorial.
19. Create a function with a default parameter.
20. Rewrite normal functions as arrow functions.

### Array Methods

21. Use `forEach()` to print all numbers.
22. Use `map()` to double numbers.
23. Use `filter()` to find even numbers.
24. Use `filter()` to find marks greater than 75.
25. Use `find()` to find a user by ID.
26. Use `some()` to check whether an array contains an even number.
27. Use `every()` to check whether all numbers are positive.
28. Use `reduce()` to calculate a total.
29. Chain `filter()` and `map()`.
30. Use `map()` on an array of objects to extract names.

### Modern JavaScript

31. Use array destructuring.
32. Use object destructuring.
33. Copy an array using spread.
34. Merge two arrays using spread.
35. Copy an object using spread.
36. Update an object using spread.
37. Create a function using the rest operator.
38. Use optional chaining.
39. Use nullish coalescing.

---

# 83. Day 2 Final Revision

At the end of Day 2, you should be comfortable reading code like this:

```javascript
const students = [

    {
        id: 1,
        name: "Sakshi",
        marks: 90
    },

    {
        id: 2,
        name: "Amit",
        marks: 75
    },

    {
        id: 3,
        name: "Rahul",
        marks: 85
    }

];

const passedStudents = students
    .filter(student => student.marks >= 80)
    .map(({ name, marks }) => ({
        name,
        marks
    }));

console.log(passedStudents);
```

Don't worry if this looks complicated initially.

Break it down:

```text
students
   ↓
array of objects
   ↓
filter()
   ↓
keep students with marks >= 80
   ↓
map()
   ↓
transform the objects
   ↓
destructuring
   ↓
extract name and marks
   ↓
new array
```

This is exactly why we are learning these concepts **step-by-step instead of memorizing shortcuts**.

---

# 🎯 What You Should Be Able to Do After Day 2

You should be able to:

* Store multiple values using arrays.
* Manipulate arrays.
* Work with objects.
* Work with arrays of objects.
* Create reusable functions.
* Understand parameters and arguments.
* Return values from functions.
* Write arrow functions.
* Use callbacks.
* Use `forEach()`.
* Use `map()`.
* Use `filter()`.
* Use `find()`.
* Use `some()`.
* Use `every()`.
* Use `reduce()`.
* Destructure arrays and objects.
* Use the spread operator.
* Use the rest operator.
* Understand optional chaining.
* Understand nullish coalescing.
* Read common modern JavaScript code.

Once these become comfortable, **Day 3 will become much easier**, because we'll take these JavaScript fundamentals and connect them to the **HTML page through the DOM**—selecting elements, changing content/styles, handling button clicks, reading forms, and performing validation.
