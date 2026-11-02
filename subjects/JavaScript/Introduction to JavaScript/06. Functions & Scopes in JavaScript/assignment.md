# Assignment: Functions in JavaScript

---

# Section 1: What Is a Function?

### 1. Why do we use functions instead of writing the same code again and again? Explain with one simple example.

Functions help us reuse code without writing it again and again.

Example:

``` 
function greet() {
    console.log("Hello Student");
}

greet();
greet();
```

### 2. List any four advantages of functions and write one line for each advantage.

1. Code Reusability: We can use the same code many times.
2. Less Code: Functions reduce repeated code.
3. Easy Debugging: Errors can be found easily.
4. Easy Maintenance: Code becomes easier to update.

### 3. Imagine you have to display a welcome message at 6 different places in your program. How will a function help you here?

We can create one function and call it six times.

```
function welcome() {
    console.log("Welcome to JavaScript");
}

welcome();
welcome();
welcome();
welcome();
welcome();
welcome();
```

### 4. Show the same code written twice without a function and once with a function.

Without Function:

```
console.log("Welcome Student");
console.log("Welcome Student");
```

With Function:

```
function welcome() {
    console.log("Welcome Student");
}

welcome();
welcome();
```

### 5. Give one real-life analogy that explains the idea of a function.

A washing machine is like a function. We give clothes and detergent as input, and it gives us clean clothes as output.

### 6. Why do functions make debugging easier? Answer in 1–2 lines.

Functions divide a program into smaller parts. We can check and fix errors in a particular function easily.

---

# Section 2: Function Declaration

### 1. Create a function declaration named displayCourse that returns "JavaScript Fundamentals". Call it and print the result.

```
function displayCourse() {
    return "JavaScript Fundamentals";
}

console.log(displayCourse());
```

### 2. Write a function declaration getStudentStatus that returns the string "Active Learner". Store the returned value in a variable and print it.

```
function getStudentStatus() {
    return "Active Learner";
}

let status = getStudentStatus();

console.log(status);
```

### 3. Write a function declaration and call it before its definition. What happens and why? Explain briefly.

```
greet();

function greet() {
    console.log("Hello Student");
}
```

Output:

```
Hello Student
```

Explanation: Function declarations are hoisted in JavaScript, so we can call them before their definition.

---

# Section 3: Function Expression

### 1. Create a function expression named showMotto that returns "Code. Learn. Grow.". Call it and print the output.

```
let showMotto = function() {
    return "Code. Learn. Grow.";
};

console.log(showMotto());
```

### 2. Write a function expression getSemester that returns the number 3. Print the value returned by the function.

```
let getSemester = function() {
    return 3;
};

console.log(getSemester());
```

### 3. Create a function expression and try to call it before writing the expression. What error do you get and why?

```
showMotto();

let showMotto = function() {
    console.log("Code. Learn. Grow.");
};
```

Output:

```
ReferenceError
```

Explanation: A function expression cannot be called before its variable is initialized.

---

# Section 4: Function Calling (Invocation)

### 1. Write a function declaration greetStudent that returns "All the best for your coding journey!". Call this function four times.

```
function greetStudent() {
    return "All the best for your coding journey!";
}

console.log(greetStudent());
console.log(greetStudent());
console.log(greetStudent());
console.log(greetStudent());
```

### 2. Create a function expression todayFocus that returns "Focus on functions today". Store the result in a variable and print that variable.

```
let todayFocus = function() {
    return "Focus on functions today";
};

let result = todayFocus();

console.log(result);
```

### 3. Write one function declaration and one function expression. Call each of them twice and print all four results.

```
function greet() {
    return "Hello Student";
}

let welcome = function() {
    return "Welcome to Coding";
};

console.log(greet());
console.log(greet());

console.log(welcome());
console.log(welcome());
```

---

# Section 5: Parameters vs Arguments

## Practical Questions

### 1. Write a function declaration subtract(a, b) that returns the difference of two numbers. Call it with arguments 50 and 18 and print the result.

```
function subtract(a, b) {
    return a - b;
}

console.log(subtract(50, 18));
```

### 2. Create a function expression greetUser(name) that returns "Welcome, " + name + "!". Call it with the argument "Aarav".

```
let greetUser = function(name) {
    return "Welcome, " + name + "!";
};

console.log(greetUser("Aarav"));
```

### 3. Write a function calculateArea(length, breadth) that returns the area of a rectangle. Call it twice with different pairs of arguments: (12, 5) and (8, 9).

```
function calculateArea(length, breadth) {
    return length * breadth;
}

console.log(calculateArea(12, 5));
console.log(calculateArea(8, 9));
```

## Theory Questions

### 4. What is the difference between a parameter and an argument? Explain with a short example.

Parameters are variables written inside the function definition. Arguments are actual values passed while calling the function.

Example:

```
function add(a, b) {
    return a + b;
}

add(10, 20);
```

Here, a and b are parameters, while 10 and 20 are arguments.

### 5. Can a function have parameters but be called without arguments? What happens in that case? Explain briefly.

Yes, a function can be called without arguments. Its parameters get the value undefined by default.

Example:

```
function greet(name) {
    console.log(name);
}

greet();
```

Output:

```
undefined
```

---

# Section 6: Return Statement

## Practical Questions

### 1. Write a function squareOfNumber(n) that returns the square of the given number. Call it with 9 and print the returned value.

```
function squareOfNumber(n) {
    return n * n;
}

console.log(squareOfNumber(9));
```

### 2. Create a function isAdult(age) that returns true if age is 18 or above, otherwise returns false. Test it with 17 and 20.

```
function isAdult(age) {
    if (age >= 18) {
        return true;
    } else {
        return false;
    }
}

console.log(isAdult(17));
console.log(isAdult(20));
```

### 3. Write a function getFullName(firstName, lastName) that returns the full name. Call it with "Rohit" and "Sharma" and print the result.

```
function getFullName(firstName, lastName) {
    return firstName + " " + lastName;
}

console.log(getFullName("Rohit", "Sharma"));
```

## Theory Questions

### 4. What does a function return if there is no return statement inside it?

If a function does not have a return statement, it returns undefined by default.

### 5. Why do we use the return statement in a function instead of just using console.log() inside the function? Explain in 2–3 lines.

Return sends the result back to the place where the function was called. We can store that result in a variable and use it again, whereas console.log() only displays the output.

---

# Section 7: Why Use Functions? (Real-World Example)

## Practical Questions

### 1. You need to calculate the total marks of three subjects for 4 different students. Write a function getTotal(m1, m2, m3) and call it four times with different marks instead of repeating the addition code.

```
function getTotal(m1, m2, m3) {
    return m1 + m2 + m3;
}

console.log(getTotal(80, 75, 90));
console.log(getTotal(70, 85, 80));
console.log(getTotal(90, 95, 85));
console.log(getTotal(65, 70, 75));
```

### 2. Create a function calculateSimpleInterest(principal, rate, time) that returns the simple interest. Use the function to find interest for two different sets of values.

```
function calculateSimpleInterest(principal, rate, time) {
    return (principal * rate * time) / 100;
}

console.log(calculateSimpleInterest(10000, 5, 2));
console.log(calculateSimpleInterest(20000, 6, 3));
```

### 3. Without using a function, write code to find the average of three numbers twice (for two students). Then rewrite the same logic using a single function findAverage(a, b, c) and call it twice.

Without Function:

```
let avg1 = (80 + 70 + 90) / 3;
console.log(avg1);

let avg2 = (60 + 75 + 85) / 3;
console.log(avg2);
```

With Function:

```
function findAverage(a, b, c) {
    return (a + b + c) / 3;
}

console.log(findAverage(80, 70, 90));
console.log(findAverage(60, 75, 85));
```

## Theory Questions

### 4. How do functions help in reducing code repetition? Explain with one real-world example.

Functions allow us to write code once and use it many times. For example, a calculator can use one addition function for different numbers.

### 5. Mention any three advantages of using functions in a program.

1. Code Reusability: We can call the same function multiple times.
2. Easy Debugging: Errors can be found and fixed easily.
3. Less Code: Functions reduce repetition and make programs shorter.
