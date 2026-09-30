

// Assignment: Introduction to Variables and Datatypes
// Part I: Variables (let, var, const)


// ==================== PART A ====================


// Q1. Personal Information
// Question: Declare variables for name, age, and city using appropriate
// variable keywords. Assign values and print all three variables.

// Answer:

let name = "Rahul";
let age = 18;
let city = "Delhi";

console.log("Name:", name);
console.log("Age:", age);
console.log("City:", city);

// Explanation: let is used to declare variables whose values can change.


// Q2. Change the Score
// Question: Create a variable score with the value 50. Change its value
// to 80 and print the final value. Use the appropriate keyword.

// Answer:

let score = 50;
score = 80;

console.log("Final Score:", score);

// Explanation: let allows us to change the value of a variable.


// Q3. Constant Value
// Question: Create a constant variable PI with the value 3.14.
// Print its value. Do not try to change the value.

// Answer:

const PI = 3.14;

console.log("Value of PI:", PI);

// Explanation: const is used when a variable should not be reassigned.


// Q4. Uninitialized Variables
// Question: Declare num1 using var and num2 using let without values.
// Print both variables. Then assign values and print them again.

// Answer:

var num1;
let num2;

console.log("Before assigning:", num1, num2);

num1 = 10;
num2 = 20;

console.log("After assigning:", num1, num2);

// Explanation: Both variables initially contain undefined.
// After assigning values, they contain 10 and 20.


// ==================== PART B ====================


// Q5. Choose the Correct Keyword
// Question: Create studentName, marks, and schoolName using appropriate
// keywords. studentName and schoolName will not change, but marks may
// change. Assign values, change marks, and print all variables.

// Answer:

const studentName = "Rahul";
let marks = 50;
const schoolName = "ABC School";

marks = 80;

console.log("Student Name:", studentName);
console.log("Marks:", marks);
console.log("School Name:", schoolName);

// Explanation: const is used for values that will not be reassigned.
// let is used for values that may change.


// Q6. Understand Scope
// Question: Declare var, let, and const variables inside an if block.
// Try to access all three variables outside the block.
// Identify which variables can be accessed.

// Answer:

if (true) {
    var a = 10;
    let b = 20;
    const c = 30;

    console.log("Inside block:", a, b, c);
}

console.log("Outside block:", a);
// console.log(b); // Error
// console.log(c); // Error

// Explanation: var can be accessed outside the if block.
// let and const are block-scoped and cannot be accessed outside it.


// Q7. Test Re-declaration
// Question: Declare a variable named user using var and declare it
// again with a different value. Repeat using let. Identify which
// declaration allows re-declaration.

// Answer:

var user = "Rahul";
var user = "Amit";

console.log("User:", user);

// let user2 = "Rahul";
// let user2 = "Amit"; // Error

// Explanation: var allows re-declaration in the same scope.
// let does not allow re-declaration in the same scope.
// The let example is commented out to prevent an error.


// Q8. Test Re-assignment
// Question: Create three variables using var, let, and const.
// Assign an initial value to each. Try to change all three values.
// Identify which variables allow re-assignment.

// Answer:

var first = 10;
let second = 20;
const third = 30;

first = 15;
second = 25;

// third = 35; // Error

console.log("Var value:", first);
console.log("Let value:", second);
console.log("Const value:", third);

// Explanation: var and let allow re-assignment.
// const does not allow re-assignment.
// The error line is commented out so the program can run.


// ==================== PART C ====================


// Q9. Predict and Explain
// Question: Without running the code, predict the output of each
// console.log() and identify which lines cause errors.
// Explain using scope, re-assignment, and variable declaration.

// Given Code:

var x = 10;

if (true) {
    var x = 20;
    let y = 30;
    const z = 40;
}

// Answer:

console.log(x); // Output: 20
// console.log(y); // Error
// console.log(z); // Error

// Explanation: x prints 20 because var is not block-scoped.
// y and z cause errors because let and const are block-scoped.
// They cannot be accessed outside the if block.


// Q10. Fix the Program
// Question: Fix the program so that it runs correctly.
// Follow the rules for initialization, re-declaration,
// re-assignment, and scope.

// Given Code:

// const name;
// let age = 20;
// let age = 25;
// if (true) {
//     var city = "Delhi";
//     let country = "India";
// }
// console.log(country);
// const score = 50;
// score = 80;


// Answer:

const personName = "Rahul";

let personAge = 20;
personAge = 25;

if (true) {
    var personCity = "Delhi";
    let country = "India";

    console.log("Country:", country);
}

console.log("Name:", personName);
console.log("Age:", personAge);
console.log("City:", personCity);

const finalScore = 50;
console.log("Score:", finalScore);

// Explanation:
// 1. const must be initialized when declared.
// 2. let can be reassigned but not redeclared in the same scope.
// 3. country must be accessed inside its block.
// 4. const cannot be reassigned.
// 5. var can be accessed outside the if block.
