
// Assignment: Introduction to Variables and Datatypes
// Part I: Variables (let, var, const)

// ==================== PART A ====================

// Q1. Personal Information
// Declare variables for name, age, and city using appropriate keywords.
// Assign values and print all three variables.

let name = "Rahul";
let age = 18;
let city = "Delhi";

console.log("Name:", name);
console.log("Age:", age);
console.log("City:", city);

// Explanation: let is used to create variables whose values can change.


// Q2. Change the Score
// Create a variable score with the value 50.
// Change its value to 80 and print the final value.

let score = 50;
score = 80;

console.log("Final Score:", score);

// Explanation: let allows us to change the value of a variable.


// Q3. Constant Value
// Create a constant variable PI with the value 3.14.
// Print its value without changing it.

const PI = 3.14;

console.log("Value of PI:", PI);

// Explanation: const is used when a variable should not be reassigned.


// Q4. Uninitialized Variables
// Declare num1 using var and num2 using let without values.
// Print both variables, assign values, and print them again.

var num1;
let num2;

console.log("Before assigning:", num1, num2);

num1 = 10;
num2 = 20;

console.log("After assigning:", num1, num2);

// Explanation: Variables declared without values contain undefined
// until a value is assigned.


// ==================== PART B ====================

// Q5. Choose the Correct Keyword
// studentName and schoolName will not change.
// marks may change. Assign values and change marks.

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
// Declare var, let, and const inside an if block.
// Try to access them outside the block.

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
// let and const are limited to the block where they are declared.


// Q7. Test Re-declaration
// Declare a variable using var twice.
// Try the same experiment using let.

var user = "Rahul";
var user = "Amit";

console.log("User:", user);

// let user2 = "Rahul";
// let user2 = "Amit"; // Error

// Explanation: var allows re-declaration in the same scope.
// let does not allow re-declaration in the same scope.
// The let example is commented out to prevent an error.


// Q8. Test Re-assignment
// Create variables using var, let, and const.
// Assign initial values and try to change them.

var first = 10;
let second = 20;
const third = 30;

first = 15;
second = 25;

// third = 35; // Error: const cannot be reassigned.

console.log("Var value:", first);
console.log("Let value:", second);
console.log("Const value:", third);

// Explanation: var and let allow re-assignment.
// const does not allow re-assignment.
// The const error is commented out so the program can run.


// ==================== PART C ====================

// Q9. Predict and Explain
// Predict the output and identify the lines that cause errors.

var x = 10;

if (true) {
    var x = 20;
    let y = 30;
    const z = 40;
}

console.log(x); // Output: 20
// console.log(y); // Error: y is block-scoped.
// console.log(z); // Error: z is block-scoped.

// Explanation: var is not limited to the if block.
// The second declaration changes x to 20.
// let and const cannot be accessed outside their block.
// The error lines are commented out so the program can run.


// Q10. Fix the Program
// Correct the errors related to initialization,
// re-declaration, re-assignment, and scope.

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
// const must be initialized when declared.
// let can be reassigned but cannot be redeclared
// in the same scope.
// country is printed inside its block.
// const cannot be reassigned.
// var can be accessed outside the if block.
