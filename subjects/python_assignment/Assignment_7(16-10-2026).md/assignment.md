# Assignment 7 – Python While Loop

## Type 1: Output Guessing

### Level 1: Understand the Basic Flow

**Q1. Simple Counting**

**Code:**
```python
i = 1

while i <= 4:
    print(i)
    i += 1
```

**Answer:**
```text
1
2
3
4
```

**Explanation:**
- Initially, `i = 1`.
- The loop runs while `i <= 4`.
- It prints the current value of `i`.
- `i += 1` increases the value by 1.
- When `i` becomes 5, the condition becomes false and the loop stops.

**Tip:** Always check the condition before every iteration.

---

**Q2. Counting by Two**

**Code:**
```python
n = 2

while n <= 8:
    print(n, end=" ")
    n += 2
```

**Answer:**
```text
2 4 6 8
```

**Explanation:**
- Starts at 2.
- Prints the value and increases it by 2.
- Values printed are 2, 4, 6 and 8.
- When `n = 10`, the condition becomes false.

**Tip:** `end=" "` prints values on the same line with spaces.

---

**Q3. Reverse Counting**

**Code:**
```python
x = 5

while x >= 1:
    print(x, end=" ")
    x -= 1
```

**Answer:**
```text
5 4 3 2 1
```

**Explanation:**
- Starts from 5.
- `x -= 1` decreases the value by 1.
- The loop stops when `x` becomes 0.

**Tip:** Use `+= 1` for increasing and `-= 1` for decreasing.

---

**Q4. The Condition Is Initially False**

**Code:**
```python
count = 7

while count < 5:
    print("Hello")
    count += 1

print("Finished")
```

**Answer:**
```text
Finished
```

**Explanation:**
- Initially, `count = 7`.
- The condition `count < 5` is false.
- Therefore, the loop never executes.
- The statement after the loop still executes.

**Important Note:** A while loop can execute zero times if its starting condition is false.

### Level 2: Track the Order of Statements

**Q5. Update Before Printing**

**Code:**
```python
i = 1

while i <= 4:
    i += 1
    print(i, end=" ")
```

**Answer:**
```text
2 3 4 5
```

**Explanation:**
The variable is increased before printing.

| Iteration | i after update | Printed |
|---|---:|---:|
| 1 | 2 | 2 |
| 2 | 3 | 3 |
| 3 | 4 | 4 |
| 4 | 5 | 5 |

The next condition check is `5 <= 4`, which is false.

**Trick:** Always follow the statement order. Updating before printing changes the output.

---

**Q6. Print After the Loop**

**Code:**
```python
n = 1

while n <= 3:
    print(n, end=" ")
    n += 1

print("Done")
```

**Answer:**
```text
1 2 3 Done
```

**Explanation:**
- The loop prints 1, 2 and 3.
- When `n = 4`, the loop stops.
- `print("Done")` is outside the loop, so it executes once after the loop.

**Tip:** Check indentation to identify statements inside and outside the loop.

---

**Q7. Two Updates in One Iteration**

**Code:**
```python
x = 1

while x < 10:
    print(x, end=" ")
    x += 2
    x += 1
```

**Answer:**
```text
1 4 7
```

**Explanation:**

Both updates happen during each iteration.

| Iteration | Printed x | After both updates |
|---|---:|---:|
| 1 | 1 | 4 |
| 2 | 4 | 7 |
| 3 | 7 | 10 |

When `x = 10`, the condition becomes false.

**Trick:** Two updates of `x += 2` and `x += 1` mean the total increase is 3.

---

**Q8. Change the Variable Before Checking Again**

**Code:**
```python
value = 10

while value > 0:
    value -= 3
    print(value, end=" ")
```

**Answer:**
```text
7 4 1 -2
```

**Explanation:**

| Iteration | Value after subtraction |
|---|---:|
| 1 | 7 |
| 2 | 4 |
| 3 | 1 |
| 4 | -2 |

The condition is checked before entering each iteration. Therefore, the loop runs when the value is 1, even though it becomes -2 inside that iteration.

The next condition check fails.

**Important:** The condition is not checked again halfway through an iteration.

### Level 3: Arithmetic and Accumulation

**Q9. Add the Counter Values**

**Code:**
```python
i = 1
total = 0

while i <= 4:
    total += i
    i += 1

print(total)
```

**Answer:**
```text
10
```

**Explanation:**

The loop adds each number to `total`.

| i | total |
|---|---:|
| 1 | 1 |
| 2 | 3 |
| 3 | 6 |
| 4 | 10 |

Final answer = 10.

**Trick:** `total += i` means `total = total + i`.

---

**Q10. Multiply During Each Iteration**

**Code:**
```python
n = 1
result = 1

while n <= 4:
    result *= 2
    n += 1

print(result)
```

**Answer:**
```text
16
```

**Explanation:**

The result is multiplied by 2 in every iteration.

| Iteration | result |
|---|---:|
| Start | 1 |
| 1 | 2 |
| 2 | 4 |
| 3 | 8 |
| 4 | 16 |

**Tip:** `result *= 2` means `result = result * 2`.

---

**Q11. Use the Remainder Operator**

**Code:**
```python
n = 11

while n > 0:
    print(n % 3, end=" ")
    n -= 4
```

**Answer:**
```text
2 1 0
```

**Explanation:**

`%` gives the remainder after division.

| n | n % 3 | Next n |
|---|---:|---:|
| 11 | 2 | 7 |
| 7 | 1 | 3 |
| 3 | 0 | -1 |

When `n = -1`, the condition `n > 0` becomes false.

**Trick:** Remember: `11 % 3 = 2`, because 3 × 3 = 9 and the remainder is 2.

---

**Q12. Integer Division**

**Code:**
```python
number = 583

while number > 0:
    print(number // 10, end=" ")
    number //= 10
```

**Answer:**
```text
58 5 0
```

**Explanation:**

`//` performs integer division.

| number | Printed value | Updated number |
|---|---:|---:|
| 583 | 58 | 58 |
| 58 | 5 | 5 |
| 5 | 0 | 0 |

When `number` becomes 0, the loop stops.

**Important Difference:**
- `% 10` extracts the last digit.
- `// 10` removes the last digit.

### Level 4: Conditions and Logical Thinking

**Q13. Print Only When a Condition Is True**

**Code:**
```python
i = 1

while i <= 6:
    if i % 2 == 0:
        print(i, end=" ")
    i += 1
```

**Answer:**
```text
2 4 6
```

**Explanation:**
- `i % 2 == 0` checks whether a number is even.
- The loop checks numbers from 1 to 6.
- Only even numbers are printed.

**Trick:** A number is even if `number % 2 == 0`.

---

**Q14. A Conditional Expression Inside a Loop**

**Code:**
```python
n = 1

while n <= 5:
    print("Even" if n % 2 == 0 else "Odd", end=" ")
    n += 1
```

**Answer:**
```text
Odd Even Odd Even Odd
```

**Explanation:**
- 1 is odd.
- 2 is even.
- 3 is odd.
- 4 is even.
- 5 is odd.

The conditional expression chooses what to print.

**Tip:** `A if condition else B` means print A when the condition is true; otherwise, print B.

---

**Q15. The Condition Changes Inside the Loop**

**Code:**
```python
x = 1

while x < 10:
    print(x, end=" ")
    x *= 2
```

**Answer:**
```text
1 2 4 8
```

**Explanation:**

| Iteration | Printed x | Updated x |
|---|---:|---:|
| 1 | 1 | 2 |
| 2 | 2 | 4 |
| 3 | 4 | 8 |
| 4 | 8 | 16 |

When `x = 16`, the condition is false.

**Trick:** `x *= 2` doubles the value each time.

---

**Q16. A Tricky Starting Value**

**Code:**
```python
i = 5

while i > 0:
    print(i, end=" ")
    i -= 2

print("Stop:", i)
```

**Answer:**
```text
5 3 1 Stop: -1
```

**Explanation:**
- Starts at 5.
- Decreases by 2 after every print.
- The values printed are 5, 3 and 1.
- After the final update, `i = -1`.
- The loop stops, and the final print statement executes.

**Important:** The final value of a variable may not be the last value printed.

### Level 5: Strings and Tricky Cases

**Q17. Build a String Repeatedly**

**Code:**
```python
i = 1
result = ""

while i <= 4:
    result += "A"
    print(result)
    i += 1
```

**Answer:**
```text
A
AA
AAA
AAAA
```

**Explanation:**
- Initially, `result` is an empty string.
- Each iteration adds one `"A"`.
- The updated string is printed every time.

**Tip:** `result += "A"` adds A to the end of the existing string.

---

**Q18. A String Variable Changes Each Time**

**Code:**
```python
word = "PY"

while len(word) < 6:
    print(word)
    word += "T"

print(word)
```

**Answer:**
```text
PY
PYT
PYTT
PYTTT
```

**Explanation:**

| Iteration | word | Length |
|---|---|---:|
| 1 | PY | 2 |
| 2 | PYT | 3 |
| 3 | PYTT | 4 |
| 4 | PYTTT | 5 |
| Stop | PYTTTT | 6 |

After the loop stops, the final `print(word)` prints `PYTTTT`.

**Correct complete output:**
```text
PY
PYT
PYTT
PYTTT
PYTTTT
```

**Important:** The last print statement is outside the loop, so it prints the final updated string.

---

**Q19. Does the Loop Run at All?**

**Code:**
```python
x = 3

while x > 10:
    print("Inside")
    x += 1

print(x)
```

**Answer:**
```text
3
```

**Explanation:**
- Initially, `x = 3`.
- The condition `3 > 10` is false.
- The loop never starts.
- The statement outside the loop prints 3.

**Tip:** Always check the initial condition first.

---

**Q20. Find the Problem**

**Code:**
```python
i = 1

while i <= 4:
    print(i, end=" ")
    i -= 1

print("Finished")
```

**Correct option: B. It prints 1 0 -1 -2 ... and continues indefinitely.**

**Explanation:**
- Initially, `i = 1`.
- The condition `i <= 4` is true.
- It prints 1 and decreases `i` to 0.
- Then it prints 0, -1, -2, and so on.
- The condition remains true because every decreasing value is still less than or equal to 4.
- Therefore, the loop never terminates.

**Important Note:** This is an infinite loop because the variable moves away from the stopping condition.

## Quick Revision Tricks – Q1 to Q20

1. `i += 1` → Increase by 1.
2. `i -= 1` → Decrease by 1.
3. `i *= 2` → Multiply by 2.
4. `i //= 10` → Remove the last digit.
5. `i % 10` → Get the last digit.
6. `print(x, end=" ")` → Print on the same line.
7. `print(x)` → Print on a new line.
8. A false starting condition → Loop executes zero times.
9. A print statement outside the loop → Executes after the loop.
10. A variable moving away from the stopping condition → May create an infinite loop.

**Exam Tip:** For output-guessing questions, make a small table with the variable's value, condition, printed output, and updated value. This makes tricky while-loop questions much easier.
