# JavaScript Assignment: Loops

# Part A: For Loop

### 1. Counting Numbers

Write a program to print numbers from 1 to 15.

```
for (let i = 1; i <= 15; i++) {
    console.log(i);
}
```

### 2. Even Numbers

Print all even numbers from 2 to 40.

```
for (let i = 2; i <= 40; i += 2) {
    console.log(i);
}
```

### 3. Odd Numbers

Print all odd numbers from 1 to 35.

```
for (let i = 1; i <= 35; i += 2) {
    console.log(i);
}
```

### 4. Saving Money

Calculate total savings after 10 days, increasing savings by ₹10 every day.

```
let total = 0;

for (let i = 1; i <= 10; i++) {
    total = total + (i * 10);
}

console.log("Total savings: ₹" + total);
```

### 5. Multiplication Table

Print the multiplication table of 12 from 1 to 10.

```
for (let i = 1; i <= 10; i++) {
    console.log("12 x " + i + " = " + (12 * i));
}
```

### 6. Daily Water Intake

Calculate the total glasses of water consumed over 7 days.

```
let total = 0;

for (let i = 1; i <= 7; i++) {
    total = total + 3;
    console.log("Day " + i + ": " + total + " glasses");
}
```

### 7. Shopping Calculation

Print the cost of buying 1 to 10 chocolates. One chocolate costs ₹15.

```
for (let i = 1; i <= 10; i++) {
    console.log(i + " chocolates = ₹" + (i * 15));
}
```

### 8. Sum of Even Numbers

Calculate the sum of even numbers between 2 and 30.

```
let sum = 0;

for (let i = 2; i <= 30; i += 2) {
    sum = sum + i;
}

console.log("Sum: " + sum);
```

### 9. Weekly Exercise

Print push-ups for 7 days, increasing by 5 every day.

```
for (let i = 1; i <= 7; i++) {
    console.log("Day " + i + ": " + (i * 5) + " push-ups");
}
```

### 10. Movie Tickets

Print ticket costs for 1 to 8 people. One ticket costs ₹150.

```
for (let i = 1; i <= 8; i++) {
    console.log(i + " people: ₹" + (i * 150));
}
```

# Part B: Additional For Loop Questions

### 1. Count Hot Days

Count how many temperatures are greater than 30°C.

```
let temp = [28, 32, 25, 40, 18, 35];
let count = 0;

for (let i = 0; i < temp.length; i++) {
    if (temp[i] > 30) {
        count++;
    }
}

console.log("Hot days: " + count);
```

### 2. Sum of Digits

Calculate the sum of digits of 4729.

```
let num = 4729;
let sum = 0;

for (; num > 0; num = Math.floor(num / 10)) {
    sum = sum + (num % 10);
}

console.log("Sum: " + sum);
```

### 3. Numbers Divisible by 3 and 5 but Not 7

Print numbers from 1 to 100 satisfying the condition.

```
for (let i = 1; i <= 100; i++) {
    if (i % 3 === 0 && i % 5 === 0 && i % 7 !== 0) {
        console.log(i);
    }
}
```

### 4. Print Consonants

Print only consonants from the string "JavaScript".

```
let str = "JavaScript";
let result = "";

for (let i = 0; i < str.length; i++) {
    let ch = str[i].toLowerCase();

    if (ch !== "a" && ch !== "e" && ch !== "i" && ch !== "o" && ch !== "u") {
        result = result + str[i];
    }
}

console.log(result);
```

### 5. Find Largest Number

Find the largest number in an array.

```
let num = [12, 45, 78, 23, 90, 34];
let max = num[0];

for (let i = 1; i < num.length; i++) {
    if (num[i] > max) {
        max = num[i];
    }
}

console.log("Largest number: " + max);
```

### 6. Perfect Number

Check whether 28 is a perfect number.

```
let num = 28;
let sum = 0;

for (let i = 1; i < num; i++) {
    if (num % i === 0) {
        sum = sum + i;
    }
}

if (sum === num) {
    console.log("Perfect Number");
} else {
    console.log("Not a Perfect Number");
}
```

### 7. Print Series

Print the series 1, 2, 4, 8, 16, 32, 64, 128.

```
let num = 1;

for (let i = 1; i <= 8; i++) {
    console.log(num);
    num = num * 2;
}
```

### 8. Fibonacci Series (Optional)

Print the first 20 Fibonacci numbers.

```
let a = 0;
let b = 1;

for (let i = 1; i <= 20; i++) {
    console.log(a);

    let c = a + b;
    a = b;
    b = c;
}
```

### 9. Average Student Marks

Calculate the average and count students scoring above average.

```
let marks = [45, 78, 90, 32, 56, 88];
let sum = 0;

for (let i = 0; i < marks.length; i++) {
    sum = sum + marks[i];
}

let avg = sum / marks.length;
let count = 0;

for (let i = 0; i < marks.length; i++) {
    if (marks[i] > avg) {
        count++;
    }
}

console.log("Average: " + avg);
console.log("Above average students: " + count);
```

### 10. Decimal to Binary (Optional)

Convert a decimal number into binary.

```
let num = 13;
let binary = "";

for (; num > 0; num = Math.floor(num / 2)) {
    binary = (num % 2) + binary;
}

console.log("Binary: " + binary);
```

# Part C-a: Break Inside a For Loop

### 1. Find Number 7

Find the first occurrence of 7 and print its index using break.

```
let num = [2, 5, 7, 9, 7];

for (let i = 0; i < num.length; i++) {
    if (num[i] === 7) {
        console.log("Index: " + i);
        break;
    }
}
```

### 2. Password Checker

Allow a maximum of 5 password attempts.

```
let correct = "1234";
let found = false;

for (let i = 1; i <= 5; i++) {
    let pass = prompt("Enter password:");

    if (pass === correct) {
        console.log("Access granted");
        found = true;
        break;
    }
}

if (found === false) {
    console.log("Account locked");
}
```

### 3. Sum Until It Exceeds 100

Print the last number added before the sum crosses 100.

```
let sum = 0;

for (let i = 1; ; i++) {
    sum = sum + i;

    if (sum > 100) {
        console.log("Last number added: " + i);
        break;
    }
}
```

### 4. Find Name Starting with S

Find the first name starting with S.

```
let names = ["Amit", "Rahul", "Sumit", "Sahil"];

for (let i = 0; i < names.length; i++) {
    if (names[i][0] === "S") {
        console.log(names[i]);
        break;
    }
}
```

### 5. Perfect Square Greater Than 20

Stop when a number is both a perfect square and greater than 20.

```
for (let i = 1; i <= 50; i++) {
    if (i > 20 && Math.sqrt(i) % 1 === 0) {
        console.log(i);
        break;
    }
}
```

# Part C-b: Continue Inside a For Loop

### 1. Skip Numbers Divisible by 4

Print numbers from 1 to 30, skipping multiples of 4.

```
for (let i = 1; i <= 30; i++) {
    if (i % 4 === 0) {
        continue;
    }

    console.log(i);
}
```

### 2. Sum of Positive Numbers

Calculate the sum of only positive numbers.

```
let num = [10, -5, 20, -3, 15];
let sum = 0;

for (let i = 0; i < num.length; i++) {
    if (num[i] < 0) {
        continue;
    }

    sum = sum + num[i];
}

console.log("Sum: " + sum);
```

### 3. Skip Spaces

Print every character of "Hello World", skipping spaces.

```
let str = "Hello World";

for (let i = 0; i < str.length; i++) {
    if (str[i] === " ") {
        continue;
    }

    console.log(str[i]);
}
```

### 4. Multiplication Table of 6

Skip rows where the product is divisible by 5.

```
for (let i = 1; i <= 12; i++) {
    let product = 6 * i;

    if (product % 5 === 0) {
        continue;
    }

    console.log("6 x " + i + " = " + product);
}
```

### 5. Eligible Voters

Print ages greater than or equal to 18.

```
let ages = [12, 18, 25, 15, 30, 17, 22];

for (let i = 0; i < ages.length; i++) {
    if (ages[i] < 18) {
        continue;
    }

    console.log(ages[i]);
}
```

# Part D: Reverse For Loop

### 1. Numbers Divisible by 3 but Not 9

Print numbers from 50 down to 1.

```
for (let i = 50; i >= 1; i--) {
    if (i % 3 === 0 && i % 9 !== 0) {
        console.log(i);
    }
}
```

### 2. Product of Odd Digits

Calculate the product of odd digits of 4729.

```
let num = 4729;
let product = 1;

for (; num > 0; num = Math.floor(num / 10)) {
    let digit = num % 10;

    if (digit % 2 !== 0) {
        product = product * digit;
    }
}

console.log("Product: " + product);
```

### 3. Reverse Consonants

Print consonants of "Programming" in reverse order.

```
let str = "Programming";
let result = "";

for (let i = str.length - 1; i >= 0; i--) {
    let ch = str[i].toLowerCase();

    if (ch !== "a" && ch !== "e" && ch !== "i" && ch !== "o" && ch !== "u") {
        result = result + str[i];
    }
}

console.log(result);
```

### 4. Fibonacci in Reverse Order

Print the first 15 Fibonacci numbers in reverse order.

```
let fib = [0, 1];

for (let i = 2; i < 15; i++) {
    fib[i] = fib[i - 1] + fib[i - 2];
}

for (let i = 14; i >= 0; i--) {
    console.log(fib[i]);
}
```

### 5. Check Palindrome Number

Check whether a number is a palindrome without converting it into a string.

```
let num = 121;
let temp = num;
let rev = 0;

for (; temp > 0; temp = Math.floor(temp / 10)) {
    rev = rev * 10 + (temp % 10);
}

if (num === rev) {
    console.log("Palindrome number");
} else {
    console.log("Not a palindrome number");
}
```

### 6. Largest Number Less Than 50

Find the largest number less than 50 using a reverse loop.

```
let num = [12, 45, 7, 23, 56, 89, 34];
let max = 0;

for (let i = num.length - 1; i >= 0; i--) {
    if (num[i] < 50 && num[i] > max) {
        max = num[i];
    }
}

console.log("Largest number: " + max);
```

### 7. Count Cold Days

Count temperatures below 30°C using a reverse loop.

```
let temp = [32, 28, 41, 19, 35, 27, 38];
let count = 0;

for (let i = temp.length - 1; i >= 0; i--) {
    if (temp[i] < 30) {
        count++;
    }
}

console.log("Cold days: " + count);
```

### 8. Decimal to Binary in Reverse Order

Convert 13 to binary and print its digits in reverse order.

```
let num = 13;
let binary = "";

for (; num > 0; num = Math.floor(num / 2)) {
    binary = binary + (num % 2);
}

console.log(binary);
```

### 9. Reverse Loop with Break

Find the first score greater than 80, starting from the end.

```
let marks = [90, 85, 70, 95, 60, 88, 75];

for (let i = marks.length - 1; i >= 0; i--) {
    if (marks[i] > 80) {
        console.log("Score: " + marks[i]);
        console.log("Index: " + i);
        break;
    }
}
```

### 10. Reverse Loop with Continue

Print numbers from 40 to 1, skipping perfect squares.

```
for (let i = 40; i >= 1; i--) {
    if (Math.sqrt(i) % 1 === 0) {
        continue;
    }

    console.log(i);
}
```

# Part E: Nested For Loop

### 1. Consecutive Number Triangle

Print a right-triangle pattern of consecutive numbers.

```
let num = 1;

for (let i = 1; i <= 4; i++) {
    let row = "";

    for (let j = 1; j <= i; j++) {
        row = row + num + " ";
        num++;
    }

    console.log(row);
}
```

### 2. Repeated Number Triangle

Print each row number repeatedly.

```
for (let i = 1; i <= 4; i++) {
    let row = "";

    for (let j = 1; j <= i; j++) {
        row = row + i + " ";
    }

    console.log(row);
}
```

### 3. Consecutive Number Triangle

Print consecutive numbers in a triangle.

```
let num = 1;

for (let i = 1; i <= 4; i++) {
    let row = "";

    for (let j = 1; j <= i; j++) {
        row = row + num + " ";
        num++;
    }

    console.log(row);
}
```

### 4. Hollow Square Pattern

Print a hollow square using stars.

```
for (let i = 1; i <= 4; i++) {
    let row = "";

    for (let j = 1; j <= 4; j++) {
        if (i === 1 || i === 4 || j === 1 || j === 4) {
            row = row + "* ";
        } else {
            row = row + "  ";
        }
    }

    console.log(row);
}
```

### 5. Alternate Symbol Triangle

Print the alternate # and $ pattern.

```
for (let i = 1; i <= 6; i++) {
    let row = "";

    for (let j = 1; j <= i; j++) {
        if (i % 2 !== 0) {
            row = row + "# ";
        } else {
            row = row + "$ ";
        }
    }

    console.log(row);
}
```

### 6. Alphabet Triangle

Print the alphabet triangle from A to E.

```
for (let i = 1; i <= 5; i++) {
    let row = "";

    for (let j = 0; j < i; j++) {
        row = row + String.fromCharCode(65 + j) + " ";
    }

    console.log(row);
}
```

### 7. Hollow Right Triangle

Print a hollow right-triangle star pattern.

```
for (let i = 1; i <= 5; i++) {
    let row = "";

    for (let j = 1; j <= i; j++) {
        if (j === 1 || j === i || i === 5) {
            row = row + "* ";
        } else {
            row = row + "  ";
        }
    }

    console.log(row);
}
```

### 8. Reverse Right-Angle Star Pattern

Print stars from 5 to 1 in reverse order.

```
for (let i = 5; i >= 1; i--) {
    let row = "";

    for (let j = 1; j <= i; j++) {
        row = row + "*";
    }

    console.log(row);
}
```

### 9. Reverse Repeated Number Pattern

Print each row number repeatedly in reverse order.

```
for (let i = 5; i >= 1; i--) {
    let row = "";

    for (let j = 1; j <= i; j++) {
        row = row + i + " ";
    }

    console.log(row);
}
```

### 10. Reverse Number Pattern

Print numbers from 1 to the row number.

```
for (let i = 5; i >= 1; i--) {
    let row = "";

    for (let j = 1; j <= i; j++) {
        row = row + j + " ";
    }

    console.log(row);
}
```

### 11. Reverse Consecutive Number Pattern

Print consecutive numbers from 15 to 1.

```
let num = 15;

for (let i = 5; i >= 1; i--) {
    let row = "";

    for (let j = 1; j <= i; j++) {
        row = row + num + " ";
        num--;
    }

    console.log(row);
}
```

### 12. Reverse Hollow Star Pattern

Print a reverse hollow right-triangle pattern.

```
for (let i = 5; i >= 1; i--) {
    let row = "";

    for (let j = 1; j <= i; j++) {
        if (i === 5 || j === 1 || j === i) {
            row = row + "* ";
        } else {
            row = row + "  ";
        }
    }

    console.log(row);
}
```

### 13. Square Without Main Diagonal

Print a 5x5 square, leaving the main diagonal empty.

```
for (let i = 1; i <= 5; i++) {
    let row = "";

    for (let j = 1; j <= 5; j++) {
        if (i === j) {
            row = row + "  ";
        } else {
            row = row + "* ";
        }
    }

    console.log(row);
}
```

### 14. Multiplication Tables with Even Products

Print multiplication tables from 1 to 5, showing only even products.

```
for (let i = 1; i <= 5; i++) {
    console.log("Table of " + i);

    for (let j = 1; j <= 10; j++) {
        let product = i * j;

        if (product % 2 === 0) {
            console.log(i + " x " + j + " = " + product);
        }
    }
}
```

### 15. Number Palindrome Pyramid

Print a symmetric number pyramid.

```
for (let i = 1; i <= 3; i++) {
    let row = "";

    for (let j = 1; j <= 3 - i; j++) {
        row = row + "  ";
    }

    for (let j = 1; j <= i; j++) {
        row = row + j + " ";
    }

    for (let j = i - 1; j >= 1; j--) {
        row = row + j + " ";
    }

    console.log(row);
}
```

# Part E: While Loop

### 1. Print Numbers

Print numbers from 1 to 10.

```
let i = 1;

while (i <= 10) {
    console.log(i);
    i++;
}
```

### 2. Sum of Natural Numbers

Calculate the sum of the first 10 natural numbers.

```
let i = 1;
let sum = 0;

while (i <= 10) {
    sum = sum + i;
    i++;
}

console.log("Sum: " + sum);
```

### 3. Multiplication Table

Print the multiplication table of 5.

```
let num = 5;
let i = 1;

while (i <= 10) {
    console.log(num + " x " + i + " = " + (num * i));
    i++;
}
```

### 4. Count the Digits

Count the digits of 58372.

```
let num = 58372;
let count = 0;

while (num > 0) {
    count++;
    num = Math.floor(num / 10);
}

console.log("Digits: " + count);
```

### 5. Reverse a Number

Reverse the number 12345.

```
let num = 12345;
let rev = 0;

while (num > 0) {
    let digit = num % 10;
    rev = rev * 10 + digit;
    num = Math.floor(num / 10);
}

console.log("Reverse: " + rev);
```

### 6. Sum of Digits

Calculate the sum of digits of 4729.

```
let num = 4729;
let sum = 0;

while (num > 0) {
    sum = sum + (num % 10);
    num = Math.floor(num / 10);
}

console.log("Sum: " + sum);
```

### 7. Print Numbers with Conditions

Print numbers divisible by 3 and 5 but not by 7.

```
let i = 1;

while (i <= 100) {
    if (i % 3 === 0 && i % 5 === 0 && i % 7 !== 0) {
        console.log(i);
    }

    i++;
}
```

### 8. Calculate Factorial

Calculate the factorial of 5.

```
let num = 5;
let fact = 1;

while (num > 0) {
    fact = fact * num;
    num--;
}

console.log("Factorial: " + fact);
```

### 9. Check Palindrome Number

Check whether 121 is a palindrome.

```
let num = 121;
let temp = num;
let rev = 0;

while (temp > 0) {
    let digit = temp % 10;
    rev = rev * 10 + digit;
    temp = Math.floor(temp / 10);
}

if (num === rev) {
    console.log("Palindrome number");
} else {
    console.log("Not a palindrome number");
}
```

### 10. Convert Decimal to Binary

Convert decimal number 13 into binary.

```
let num = 13;
let binary = "";

while (num > 0) {
    let rem = num % 2;
    binary = rem + binary;
    num = Math.floor(num / 2);
}

console.log("Binary: " + binary);
```

# Part F: Do-While Loop

### 1. Print Numbers in Reverse

Print numbers from 10 down to 1.

```
let i = 10;

do {
    console.log(i);
    i--;
} while (i >= 1);
```

### 2. Print Even Numbers

Print even numbers between 1 and 20.

```
let i = 2;

do {
    console.log(i);
    i += 2;
} while (i <= 20);
```

### 3. Sum of Natural Numbers

Calculate the sum of the first 5 natural numbers.

```
let n = 5;
let i = 1;
let sum = 0;

do {
    sum = sum + i;
    i++;
} while (i <= n);

console.log("Sum: " + sum);
```

### 4. Product of Digits

Calculate the product of digits of 234.

```
let num = 234;
let product = 1;

do {
    product = product * (num % 10);
    num = Math.floor(num / 10);
} while (num > 0);

console.log("Product: " + product);
```

### 5. Find the First Digit

Find the leftmost digit of 58372.

```
let num = 58372;

do {
    if (num < 10) {
        break;
    }

    num = Math.floor(num / 10);
} while (true);

console.log("First digit: " + num);
```

### 6. Calculate a Power

Calculate 3 raised to the power 4.

```
let base = 3;
let power = 4;
let result = 1;
let i = 1;

if (power === 0) {
    result = 1;
} else {
    do {
        result = result * base;
        i++;
    } while (i <= power);
}

console.log("Answer: " + result);
```

### 7. Print Multiples with Conditions

Print numbers divisible by 4 but not by 8.

```
let i = 1;

do {
    if (i % 4 === 0 && i % 8 !== 0) {
        console.log(i);
    }

    i++;
} while (i <= 100);
```

### 8. Check a Palindrome Number

Check whether 1221 is a palindrome.

```
let num = 1221;
let temp = num;
let rev = 0;

do {
    let digit = temp % 10;
    rev = rev * 10 + digit;
    temp = Math.floor(temp / 10);
} while (temp > 0);

if (num === rev) {
    console.log("Palindrome number");
} else {
    console.log("Not a palindrome number");
}
```

### 9. Find Greatest Common Divisor (GCD)

Find the GCD of 48 and 18.

```
let a = 48;
let b = 18;
let rem;

do {
    rem = a % b;
    a = b;
    b = rem;
} while (b !== 0);

console.log("GCD: " + a);
```

### 10. Convert Decimal to Binary

Convert decimal number 13 into binary. Handle 0 correctly.

```
let num = 13;
let binary = "";

if (num === 0) {
    binary = "0";
} else {
    do {
        let rem = num % 2;
        binary = rem + binary;
        num = Math.floor(num / 2);
    } while (num > 0);
}

console.log("Binary: " + binary);
```
