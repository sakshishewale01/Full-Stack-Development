Java Script is Case - Sensetive language .Always write the keywords are in same format(Specially, String-S always Capital)

# 📌 Day 1 Topics

```text
1. JavaScript Basics
2. Variables
3. Data Types
4. Type Checking
5. Type Conversion
6. Operators
7. Conditions
8. Truthy & Falsy Values
9. Loops
10. break & continue
11. Template Literals
12. Common Interview Questions
````

---

# 1. What is JavaScript?

JavaScript is a high-level, dynamically typed programming language mainly used to add logic and interactivity to web applications.

It can be used for:

```text
Frontend  → React.js
Backend   → Node.js
APIs      → Express.js
Database  → MySQL / MongoDB
```

Basic web development:

```text
HTML        → Structure
CSS         → Styling
JavaScript  → Logic + Behaviour
```

---

# 2. How to Include JavaScript in HTML

## Internal JavaScript

```html
<script>

    console.log("Hello JavaScript");

</script>
```

## External JavaScript

HTML:

```html
<script src="script.js"></script>
```

JavaScript:

```javascript
console.log("Hello JavaScript");
```

### Best Practice

Use an external JavaScript file for projects.

---

# 3. console.log()

Used to print information to the browser console.

```javascript
console.log("Hello");

console.log(100);

console.log(10 + 20);
```

Output:

```text
Hello
100
30
```

### Interview Point

`console.log()` is commonly used for:

* Debugging
* Checking values
* Understanding program execution

---

# 4. Comments

## Single-line

```javascript
// This is a comment
```

## Multi-line

```javascript
/*
   This is
   a multi-line
   comment
*/
```

Comments are ignored during program execution.

---

# 5. Variables

A variable is a named storage location used to store data.

JavaScript provides:

```text
let
const
var
```

---

# 6. let

Used when the value may change.

```javascript
let age = 19;

age = 20;

console.log(age);
```

Output:

```text
20
```

---

# 7. const

Used when a variable should not be reassigned.

```javascript
const pi = 3.14;
```

This is invalid:

```javascript
const pi = 3.14;

pi = 4;
```

---

# 8. var

`var` is the older way of declaring variables.

```javascript
var name = "Sakshi";
```

Modern JavaScript generally prefers:

```javascript
let
const
```

over `var`.

---

# 9. let vs const vs var

| Feature                         | var   | let | const |
| ------------------------------- | ----- | --- | ----- |
| Reassignment                    | Yes   | Yes | No    |
| Block scoped                    | No    | Yes | Yes   |
| Modern recommendation           | Avoid | Yes | Yes   |
| Can be redeclared in same scope | Yes   | No  | No    |

### Best Practice

Use:

```javascript
const
```

by default.

Use:

```javascript
let
```

when the value needs to change.

Avoid `var` in modern JavaScript.

---

# 10. Variable Naming

Use meaningful names.

Good:

```javascript
let studentName = "Sakshi";

let totalMarks = 90;

let userAge = 20;
```

Bad:

```javascript
let x = "Sakshi";

let a = 90;

let y = 20;
```

---

# 11. camelCase

JavaScript commonly uses camelCase.

```javascript
let firstName = "Sakshi";

let lastName = "Shewale";

let totalMarks = 95;

let studentAge = 20;
```

---

# 12. JavaScript Data Types

Important JavaScript data types:

```text
String
Number
Boolean
Undefined
Null
Object
Array
```

For Day 1, focus mainly on:

```text
String
Number
Boolean
Undefined
Null
```

---

# 13. String

Used for text.

```javascript
let name = "Sakshi";

let city = "Pune";
```

Strings can use:

```javascript
"Hello"
'Hello'
`Hello`
```

---

# 14. Number

JavaScript uses the `Number` type for integers and decimal numbers.

```javascript
let age = 19;

let price = 250;

let percentage = 89.5;
```

---

# 15. Boolean

Boolean has two values:

```javascript
true
false
```

Example:

```javascript
let isStudent = true;

let isLoggedIn = false;
```

Used heavily in conditions.

---

# 16. Undefined

A variable declared without a value has `undefined`.

```javascript
let name;

console.log(name);
```

Output:

```text
undefined
```

---

# 17. Null

`null` represents an intentionally empty value.

```javascript
let selectedUser = null;
```

Meaning:

```text
There is currently no selected user.
```

---

# 18. typeof

Used to check the type of a value.

```javascript
console.log(typeof "Hello");
console.log(typeof 100);
console.log(typeof true);
```

Output:

```text
string
number
boolean
```

Example:

```javascript
let age = 20;

console.log(typeof age);
```

Output:

```text
number
```

---

# 19. Important typeof Questions

```javascript
typeof "Hello"
```

Result:

```text
string
```

```javascript
typeof 10
```

Result:

```text
number
```

```javascript
typeof true
```

Result:

```text
boolean
```

```javascript
typeof undefined
```

Result:

```text
undefined
```

### Important Interview Question

What is:

```javascript
typeof null
```

Answer:

```text
object
```

This is a historical behavior/quirk of JavaScript.

---

# 20. Type Conversion

Type conversion means changing one data type into another.

Common functions:

```text
Number()
String()
Boolean()
parseInt()
parseFloat()
```

---

# 21. Number()

Converts a value into a number.

```javascript
let age = Number("20");

console.log(age);

console.log(typeof age);
```

Output:

```text
20
number
```

---

# 22. String()

Converts a value into a string.

```javascript
let age = 20;

let result = String(age);

console.log(typeof result);
```

Output:

```text
string
```

---

# 23. Boolean()

Converts a value into boolean.

```javascript
Boolean(1);
```

Result:

```text
true
```

```javascript
Boolean(0);
```

Result:

```text
false
```

---

# 24. parseInt()

Converts a value into an integer.

```javascript
let age = parseInt("20");

console.log(age);
```

Output:

```text
20
```

---

# 25. parseFloat()

Converts a value into a decimal number.

```javascript
let price = parseFloat("99.50");

console.log(price);
```

Output:

```text
99.5
```

---

# 26. prompt()

Used to take input from the user in the browser.

```javascript
let name = prompt("Enter your name:");

console.log(name);
```

### Important

`prompt()` returns input as a **string**.

Therefore:

```javascript
let age = prompt("Enter age:");

console.log(typeof age);
```

returns:

```text
string
```

For numeric input:

```javascript
let age = Number(prompt("Enter age:"));
```

---

# 27. Arithmetic Operators

Used for mathematical operations.

| Operator | Meaning        |
| -------- | -------------- |
| `+`      | Addition       |
| `-`      | Subtraction    |
| `*`      | Multiplication |
| `/`      | Division       |
| `%`      | Modulus        |
| `++`     | Increment      |
| `--`     | Decrement      |

Example:

```javascript
let a = 10;
let b = 5;

console.log(a + b);
console.log(a - b);
console.log(a * b);
console.log(a / b);
console.log(a % b);
```

---

# 28. Modulus %

Returns the remainder.

```javascript
console.log(10 % 3);
```

Output:

```text
1
```

### Common Use

Checking even or odd:

```javascript
let number = 10;

if (number % 2 === 0) {

    console.log("Even");

} else {

    console.log("Odd");

}
```

---

# 29. Increment and Decrement

## Increment

```javascript
let count = 5;

count++;

console.log(count);
```

Output:

```text
6
```

## Decrement

```javascript
let count = 5;

count--;

console.log(count);
```

Output:

```text
4
```

---

# 30. Assignment Operators

| Operator | Example  | Equivalent  |
| -------- | -------- | ----------- |
| `=`      | `x = 5`  | Assign      |
| `+=`     | `x += 5` | `x = x + 5` |
| `-=`     | `x -= 5` | `x = x - 5` |
| `*=`     | `x *= 5` | `x = x * 5` |
| `/=`     | `x /= 5` | `x = x / 5` |

Example:

```javascript
let x = 10;

x += 5;

console.log(x);
```

Output:

```text
15
```

---

# 31. Comparison Operators

Comparison operators return:

```text
true
false
```

| Operator | Meaning               |
| -------- | --------------------- |
| `>`      | Greater than          |
| `<`      | Less than             |
| `>=`     | Greater than or equal |
| `<=`     | Less than or equal    |
| `==`     | Loose equality        |
| `===`    | Strict equality       |
| `!=`     | Loose inequality      |
| `!==`    | Strict inequality     |

---

# 32. == vs ===

This is an important interview question.

## ==

Performs type conversion if necessary.

```javascript
5 == "5"
```

Result:

```text
true
```

## ===

Checks both value and type.

```javascript
5 === "5"
```

Result:

```text
false
```

Because:

```text
5   → number
"5" → string
```

### Best Practice

Prefer:

```javascript
===
!==
```

over:

```javascript
==
!=
```

---

# 33. Logical Operators

Three important logical operators:

```text
&&
||
!
```

---

# 34. AND &&

Returns true when both conditions are true.

```javascript
let age = 20;

let hasID = true;

console.log(age >= 18 && hasID);
```

Result:

```text
true
```

---

# 35. OR ||

Returns true if at least one condition is true.

```javascript
let isStudent = true;

let isEmployee = false;

console.log(isStudent || isEmployee);
```

Result:

```text
true
```

---

# 36. NOT !

Reverses a boolean value.

```javascript
let isLoggedIn = true;

console.log(!isLoggedIn);
```

Result:

```text
false
```

---

# 37. Conditions

Conditions allow JavaScript to make decisions.

Main conditional statements:

```text
if
if-else
else-if
switch
ternary
```

---

# 38. if

Syntax:

```javascript
if (condition) {

    // code

}
```

Example:

```javascript
let age = 20;

if (age >= 18) {

    console.log("Adult");

}
```

---

# 39. if-else

```javascript
let marks = 30;

if (marks >= 40) {

    console.log("Pass");

} else {

    console.log("Fail");

}
```

Output:

```text
Fail
```

---

# 40. else-if

Used when multiple conditions need to be checked.

```javascript
let marks = 85;

if (marks >= 90) {

    console.log("A+");

} else if (marks >= 75) {

    console.log("A");

} else if (marks >= 60) {

    console.log("B");

} else {

    console.log("C");

}
```

---

# 41. Nested if

An `if` statement inside another `if`.

```javascript
let age = 20;

let hasID = true;

if (age >= 18) {

    if (hasID) {

        console.log("Entry allowed");

    }

}
```

Avoid unnecessary deep nesting.

---

# 42. Ternary Operator

Short form of simple `if-else`.

Syntax:

```javascript
condition ? valueIfTrue : valueIfFalse;
```

Example:

```javascript
let age = 20;

let result = age >= 18 ? "Adult" : "Minor";

console.log(result);
```

Output:

```text
Adult
```

### Common in React

Ternary operators are frequently used for conditional rendering.

---

# 43. switch

Used when one value has multiple possible cases.

```javascript
let day = 2;

switch (day) {

    case 1:
        console.log("Monday");
        break;

    case 2:
        console.log("Tuesday");
        break;

    case 3:
        console.log("Wednesday");
        break;

    default:
        console.log("Invalid day");

}
```

---

# 44. break in switch

`break` stops execution of the switch.

```javascript
case 1:

    console.log("Monday");

    break;
```

Without `break`, execution can continue into the next cases.

---

# 45. Truthy and Falsy Values

JavaScript treats certain values as false in boolean contexts.

Important falsy values:

```text
false
0
""
null
undefined
NaN
```

Almost everything else is truthy.

Example:

```javascript
let name = "";

if (name) {

    console.log("Name exists");

} else {

    console.log("Name is empty");

}
```

Output:

```text
Name is empty
```

---

# 46. Loops

Loops execute code repeatedly.

Main loops:

```text
for
while
do...while
```

---

# 47. for Loop

Used when the number of repetitions is known.

Syntax:

```javascript
for (initialization; condition; update) {

    // code

}
```

Example:

```javascript
for (let i = 1; i <= 5; i++) {

    console.log(i);

}
```

Output:

```text
1
2
3
4
5
```

---

# 48. How for Loop Works

Example:

```javascript
for (let i = 1; i <= 5; i++) {

    console.log(i);

}
```

Execution:

```text
1. let i = 1
2. Check i <= 5
3. Execute code
4. i++
5. Check condition again
6. Repeat
```

---

# 49. while Loop

Used when repetition depends mainly on a condition.

```javascript
let i = 1;

while (i <= 5) {

    console.log(i);

    i++;

}
```

Output:

```text
1
2
3
4
5
```

### Important

Always make sure the condition eventually becomes false.

---

# 50. do...while

The code executes at least once.

```javascript
let i = 1;

do {

    console.log(i);

    i++;

} while (i <= 5);
```

---

# 51. for vs while vs do...while

| Loop         | Use                         |
| ------------ | --------------------------- |
| `for`        | Known number of repetitions |
| `while`      | Condition-based repetition  |
| `do...while` | Must execute at least once  |

---

# 52. break

Stops the loop immediately.

```javascript
for (let i = 1; i <= 10; i++) {

    if (i === 5) {

        break;

    }

    console.log(i);

}
```

Output:

```text
1
2
3
4
```

---

# 53. continue

Skips the current iteration.

```javascript
for (let i = 1; i <= 5; i++) {

    if (i === 3) {

        continue;

    }

    console.log(i);

}
```

Output:

```text
1
2
4
5
```

---

# 54. Template Literals

Double quotes (") treat everything inside them as plain text, so they cannot read variables or expressions. Backticks (`) trigger special powers that allow JavaScript to process variables inside ${} and format multi-line text [link1].

Template literals use backticks:

```javascript
`
`
```

They allow variables to be inserted using:

```javascript
${variable}
```

Example:

```javascript
let name = "Sakshi";

let age = 20;

console.log(`My name is ${name} and I am ${age} years old.`);
```

Output:

```text
My name is Sakshi and I am 20 years old.
```

### Advantage

Cleaner than string concatenation.

---

# 55. String Concatenation

Traditional method:

```javascript
let firstName = "Sakshi";

let lastName = "Shewale";

console.log(firstName + " " + lastName);
```

Modern approach:

```javascript
console.log(`${firstName} ${lastName}`);
```

Template literals are generally easier to read.

---

# 56. Mini Program — Even or Odd

```javascript
let number = Number(prompt("Enter a number:"));

if (number % 2 === 0) {

    console.log("Even");

} else {

    console.log("Odd");

}
```

Concepts:

```text
prompt()
Number()
%
if-else
===
```

---

# 57. Mini Program — Positive, Negative or Zero

```javascript
let number = Number(prompt("Enter a number:"));

if (number > 0) {

    console.log("Positive");

} else if (number < 0) {

    console.log("Negative");

} else {

    console.log("Zero");

}
```

---

# 58. Mini Program — Largest of Three Numbers

```javascript
let a = Number(prompt("Enter first number:"));

let b = Number(prompt("Enter second number:"));

let c = Number(prompt("Enter third number:"));

if (a >= b && a >= c) {

    console.log("A is largest");

} else if (b >= a && b >= c) {

    console.log("B is largest");

} else {

    console.log("C is largest");

}
```

---

# 59. Mini Program — Multiplication Table

```javascript
let number = Number(prompt("Enter a number:"));

for (let i = 1; i <= 10; i++) {

    console.log(`${number} × ${i} = ${number * i}`);

}
```

---

# 60. Mini Program — Factorial

```javascript
let number = Number(prompt("Enter a number:"));

let factorial = 1;

for (let i = 1; i <= number; i++) {

    factorial *= i;

}

console.log(`Factorial = ${factorial}`);
```

Example:

```text
5! = 120
```

---

# 61. Mini Program — Simple Login

```javascript
const correctUsername = "sakshi";

const correctPassword = "12345";

let username = prompt("Enter username:");

let password = prompt("Enter password:");

if (
    username === correctUsername &&
    password === correctPassword
) {

    console.log("Login successful");

} else {

    console.log("Invalid username or password");

}
```

Concepts:

```text
const
let
prompt()
===
&&
if-else
```

---

# 62. Mini Program — Grade Calculator

```javascript
let marks = Number(prompt("Enter marks:"));

if (marks >= 90) {

    console.log("Grade A+");

} else if (marks >= 80) {

    console.log("Grade A");

} else if (marks >= 70) {

    console.log("Grade B");

} else if (marks >= 60) {

    console.log("Grade C");

} else if (marks >= 40) {

    console.log("Grade D");

} else {

    console.log("Fail");

}
```

---

# 63. Interview Questions

## Q1. What is JavaScript?

JavaScript is a high-level programming language used to create dynamic and interactive web applications. It can also be used on the backend using Node.js.

---

## Q2. Difference between let, const and var?

```text
var   → Function scoped, older syntax
let   → Block scoped, reassignable
const → Block scoped, cannot be reassigned
```

Modern JavaScript prefers `let` and `const`.

---

## Q3. What are JavaScript primitive data types?

Important primitive types include:

```text
string
number
bigint
boolean
undefined
symbol
null
```

---

## Q4. What is dynamic typing?

JavaScript is dynamically typed because a variable does not have to be declared with a fixed data type.

Example:

```javascript
let value = 10;

value = "Hello";
```

The variable can hold different types at different times.

---

## Q5. Difference between == and ===?

```text
==  → Loose equality
=== → Strict equality
```

Example:

```javascript
5 == "5"     // true

5 === "5"    // false
```

Prefer `===`.

---

## Q6. What is type coercion?

Type coercion is the conversion of a value from one type to another, automatically or explicitly.

Example:

```javascript
"5" + 2
```

Result:

```text
"52"
```

because `2` is converted to a string for the `+` operation.

---

## Q7. What is the difference between null and undefined?

```text
undefined → Value has not been assigned
null      → Intentionally empty value
```

Example:

```javascript
let a;

let b = null;
```

---

## Q8. What is typeof?

`typeof` is an operator used to determine the type of a value.

```javascript
typeof "Hello"
```

Result:

```text
string
```

---

## Q9. What is a truthy value?

A truthy value is a value that behaves like `true` in a boolean context.

Example:

```javascript
if ("Hello") {

    console.log("Truthy");

}
```

---

## Q10. What are falsy values?

Important falsy values:

```text
false
0
""
null
undefined
NaN
```

---

## Q11. What is a loop?

A loop repeatedly executes a block of code while a condition is satisfied.

Examples:

```text
for
while
do...while
```

---

## Q12. Difference between for and while?

Use `for` when the number of iterations is generally known.

Use `while` when repetition is primarily controlled by a condition.

---

## Q13. What does break do?

`break` immediately terminates a loop or switch.

---

## Q14. What does continue do?

`continue` skips the current iteration and moves to the next iteration.

---

## Q15. What is a ternary operator?

A compact way of writing a simple `if-else`.

```javascript
let result = age >= 18 ? "Adult" : "Minor";
```

---

## Q16. What is template literal?

Template literals are strings enclosed in backticks that allow embedded expressions.

```javascript
let name = "Sakshi";

console.log(`Hello ${name}`);
```

---

## Q17. What does prompt() return?

`prompt()` normally returns user input as a string.

Therefore:

```javascript
let age = prompt("Age:");

typeof age
```

returns:

```text
string
```

---

## Q18. How do you convert prompt input into a number?

```javascript
let age = Number(prompt("Enter age:"));
```

---

## Q19. Why do we use strict equality?

`===` checks both value and data type, making comparisons more predictable.

---

## Q20. Why is var generally avoided?

Because `var` has function scope and has historical behaviors such as hoisting/redeclaration that can make modern code harder to reason about.

Modern JavaScript generally uses:

```text
const
let
```

---

# 64. Quick Syntax Sheet

## Variable

```javascript
let age = 20;

const name = "Sakshi";
```

## Output

```javascript
console.log("Hello");
```

## Input

```javascript
let name = prompt("Enter name:");
```

## Number Input

```javascript
let age = Number(prompt("Enter age:"));
```

## Condition

```javascript
if (condition) {

} else {

}
```

## Multiple Conditions

```javascript
if (condition) {

} else if (condition) {

} else {

}
```

## Ternary

```javascript
condition ? trueValue : falseValue;
```

## Switch

```javascript
switch (value) {

    case 1:
        // code
        break;

    default:
        // code

}
```

## for Loop

```javascript
for (let i = 0; i < 10; i++) {

}
```

## while Loop

```javascript
while (condition) {

}
```

## do...while

```javascript
do {

} while (condition);
```

---

# 65. Operator Cheat Sheet

```text
Arithmetic
+   -   *   /   %   ++   --

Assignment
=   +=   -=   *=   /=

Comparison
>   <   >=   <=   ==   ===   !=   !==

Logical
&&   ||   !

Ternary
? :
```

---

# 66. Day 1 One-Minute Revision

Before an interview, remember:

```text
Variables
    ↓
const by default
let when reassignment is needed
avoid var

Data Types
    ↓
String
Number
Boolean
Undefined
Null
Object
Array

Type Checking
    ↓
typeof

Type Conversion
    ↓
Number()
String()
Boolean()
parseInt()
parseFloat()

Operators
    ↓
Arithmetic
Assignment
Comparison
Logical

Equality
    ↓
Prefer === over ==

Conditions
    ↓
if
else-if
else
switch
ternary

Loops
    ↓
for
while
do...while

Loop Control
    ↓
break
continue

Strings
    ↓
Template literals
`${value}`
```

---

# 67. Day 1 Interview Must-Know

If you have limited time before an interview, revise these first:

### ⭐ High Priority

```text
let vs const vs var
Primitive data types
typeof
== vs ===
Type coercion
Truthy and falsy
if / else-if / else
switch
for loop
while loop
break / continue
Template literals
Number() conversion
```

---

# 68. Day 1 Completion Checklist

* [x] JavaScript Basics
* [x] console.log()
* [x] Comments
* [x] Variables
* [x] let
* [x] const
* [x] var
* [x] Data Types
* [x] typeof
* [x] Type Conversion
* [x] prompt()
* [x] Arithmetic Operators
* [x] Assignment Operators
* [x] Comparison Operators
* [x] Logical Operators
* [x] if
* [x] if-else
* [x] else-if
* [x] switch
* [x] Ternary Operator
* [x] Truthy & Falsy
* [x] for Loop
* [x] while Loop
* [x] do...while Loop
* [x] break
* [x] continue
* [x] Template Literals
* [x] Basic Programming Problems

---

# 69. What's Next?

## JavaScript Day 2

```text
Arrays
    ↓
Objects
    ↓
Functions
    ↓
Arrow Functions
    ↓
Array Methods
    ↓
Object Methods
    ↓
Destructuring
    ↓
Spread Operator
    ↓
Rest Operator
    ↓
Modern JavaScript
```

These concepts are especially important before moving to:

```text
JavaScript
    ↓
DOM
    ↓
APIs
    ↓
React.js
    ↓
Node.js
    ↓
Express.js
    ↓
Database
    ↓
Full-Stack Projects
```

---

# 🚀 Final Note

Do not try to memorize JavaScript syntax word-for-word.

Instead, understand:

```text
What does it do?
Why do we use it?
When should we use it?
How does it behave?
```

The best way to revise JavaScript is:

```text
Read
 ↓
Understand
 ↓
Write from memory
 ↓
Run
 ↓
Debug
 ↓
Solve problems
```

---