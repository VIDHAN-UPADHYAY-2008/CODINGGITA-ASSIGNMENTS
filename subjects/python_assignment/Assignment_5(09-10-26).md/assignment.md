# Assignment 5 — Single for Loop

## Q1. Predict the Loop Values
```python
for i in range(2, 15, 3):
    print(i)
```
Output:
```text
2
5
8
11
14
```

## Q2. Reverse range()
```python
for i in range(15, 2, -3):
    print(i)
```
Output:
```text
15
12
9
6
3
```

## Q3. How Many Iterations?
```python
for i in range(4, 31, 5):
    print(i)
```
Output: `4, 9, 14, 19, 24, 29` — 6 iterations.

## Q4. Correct the Boundary
```python
for i in range(3, 19, 3):
    print(i)
```

## Q5. Number and Distance from 20
```python
for i in range(5, 11):
    print(i, 20-i)
```

## Q6. Number, Square and Cube
```python
for i in range(1, 7):
    print(i, i**2, i**3)
```

## Q7. Sum of Numbers in a Range
```python
a, b = map(int, input().split())
total = 0
for i in range(a, b+1):
    total += i
print(total)
```

## Q8. Count Multiples of 3
```python
n = int(input())
count = 0
for i in range(1, n+1):
    if i % 3 == 0:
        count += 1
print(count)
```

## Q9. Sum of Multiples of 4
```python
n = int(input())
total = 0
for i in range(1, n+1):
    if i % 4 == 0:
        total += i
print(total)
```

## Q10. Count Numbers Divisible by 3 and 5
```python
n = int(input())
count = 0
for i in range(1, n+1):
    if i % 3 == 0 and i % 5 == 0:
        count += 1
print(count)
```

## Q11. Sum Except Multiples of 3
```python
n = int(input())
total = 0
for i in range(1, n+1):
    if i % 3 != 0:
        total += i
print(total)
```

## Q12. Count Even and Odd
```python
n = int(input())
even = 0
odd = 0
for i in range(1, n+1):
    if i % 2 == 0:
        even += 1
    else:
        odd += 1
print("Even =", even, "Odd =", odd)
```

## Q13. Running Sum
```python
n = int(input())
total = 0
for i in range(1, n+1):
    total += i
    print(total)
```

## Q14. Running Product
```python
n = int(input())
product = 1
for i in range(1, n+1):
    product *= i
    print(product)
```

## Q15. Factorial
```python
n = int(input())
fact = 1
for i in range(1, n+1):
    fact *= i
print(fact)
```

## Q16. Factorials from 1 to N
```python
n = int(input())
fact = 1
for i in range(1, n+1):
    fact *= i
    print(str(i) + "! =", fact)
```

## Q17. Product of Even Numbers
```python
n = int(input())
product = 1
for i in range(2, n+1, 2):
    product *= i
print(product)
```

## Q18. Product of Odd Numbers
```python
n = int(input())
product = 1
for i in range(1, n+1, 2):
    product *= i
print(product)
```

## Q19. Even Double Factorial
```python
n = int(input())
product = 1
for i in range(2, n+1, 2):
    product *= i
print(product)
```

## Q20. Sum of Squares
```python
n = int(input())
total = 0
for i in range(1, n+1):
    total += i**2
print(total)
```

## Q21. Sum of Cubes
```python
n = int(input())
total = 0
for i in range(1, n+1):
    total += i**3
print(total)
```

## Q22. Factorial-Based Sum
```python
n = int(input())
fact = 1
total = 0
for i in range(1, n+1):
    fact *= i
    total += fact
print(total)
```

## Q23. Count Digits Without String Conversion
```python
n = int(input())
count = 0
for i in range(100):
    if n > 0:
        count += 1
        n //= 10
print(count)
```

## Q24. Sum of Digits
```python
n = int(input())
total = 0
for i in range(100):
    if n > 0:
        total += n % 10
        n //= 10
print(total)
```

## Q25. Product of Digits
```python
n = int(input())
product = 1
for i in range(100):
    if n > 0:
        product *= n % 10
        n //= 10
print(product)
```

## Q26. Count Even Digits
```python
n = int(input())
count = 0
for i in range(100):
    if n > 0:
        if (n % 10) % 2 == 0:
            count += 1
        n //= 10
print(count)
```

## Q27. Sum of Even Digits
```python
n = int(input())
total = 0
for i in range(100):
    if n > 0:
        d = n % 10
        if d % 2 == 0:
            total += d
        n //= 10
print(total)
```

## Q28. Largest Digit Without max()
```python
n = int(input())
largest = 0
for i in range(100):
    if n > 0:
        d = n % 10
        if d > largest:
            largest = d
        n //= 10
print(largest)
```

## Q29. Smallest Digit Without min()
```python
n = int(input())
smallest = 9
for i in range(100):
    if n > 0:
        d = n % 10
        if d < smallest:
            smallest = d
        n //= 10
print(smallest)
```

## Q30. Reverse a Number
```python
n = int(input())
rev = 0
for i in range(100):
    if n > 0:
        rev = rev * 10 + n % 10
        n //= 10
print(rev)
```

## Q31. Palindrome Number
```python
n = int(input())
original = n
rev = 0
for i in range(100):
    if n > 0:
        rev = rev * 10 + n % 10
        n //= 10
if original == rev:
    print("Palindrome")
else:
    print("Not Palindrome")
```

## Q32. Count a Specific Digit
```python
n, target = map(int, input().replace(",", " ").split())
count = 0
for i in range(100):
    if n > 0:
        if n % 10 == target:
            count += 1
        n //= 10
print(count)
```

## Q33. First Digit
```python
n = int(input())
for i in range(100):
    if n >= 10:
        n //= 10
print(n)
```

## Q34. Difference Between Largest and Smallest
```python
n = int(input())
largest = 0
smallest = 9
for i in range(100):
    if n > 0:
        d = n % 10
        if d > largest:
            largest = d
        if d < smallest:
            smallest = d
        n //= 10
print(largest-smallest)
```

## Q35. Digit Position
```python
n = int(input())
pos = 1
for i in range(100):
    if n > 0:
        print(n % 10, pos)
        n //= 10
        pos += 1
```

## Q36. Armstrong Number
```python
n = int(input())
original = n
total = 0
for i in range(3):
    d = n % 10
    total += d**3
    n //= 10
if total == original:
    print("Armstrong Number")
else:
    print("Not Armstrong Number")
```

## Q37. Characters with Index
```python
s = input()
for i in range(len(s)):
    print(i, s[i])
```

## Q38. Count Characters Without len()
```python
s = input()
count = 0
for ch in s:
    count += 1
print(count)
```

## Q39. Count Vowels and Consonants
```python
s = input()
vowels = 0
consonants = 0
for ch in s.lower():
    if ch in "aeiou":
        vowels += 1
    elif ch.isalpha():
        consonants += 1
print("Vowels =", vowels, "Consonants =", consonants)
```

## Q40. Character Frequency
```python
s, target = input().replace(",", " ").split()
count = 0
for ch in s:
    if ch == target:
        count += 1
print(count)
```

## Q41. First Occurrence Position
```python
s, target = input().replace(",", " ").split()
pos = -1
for i in range(len(s)):
    if s[i] == target and pos == -1:
        pos = i
if pos == -1:
    print("Not Found")
else:
    print(pos)
```

## Q42. Count Uppercase and Lowercase
```python
s = input()
upper = 0
lower = 0
for ch in s:
    if ch.isupper():
        upper += 1
    elif ch.islower():
        lower += 1
print("Uppercase =", upper, "Lowercase =", lower)
```

## Q43. Character Code Analyzer
```python
s = input()
for ch in s:
    print(ch, ord(ch))
```

## Q44. String Without Vowels
```python
s = input()
result = ""
for ch in s:
    if ch.lower() not in "aeiou":
        result += ch
print(result)
```

## Q45. Middle Character
```python
s = input()
print(s[len(s)//2])
```

## Q46. First Half and Second Half
```python
s = input()
mid = len(s)//2
print("First Half:", s[:mid])
print("Second Half:", s[mid:])
```

## Q47. Split String Without Slicing
```python
s = input()
mid = len(s)//2
first = ""
middle = ""
second = ""
for i in range(len(s)):
    if i < mid:
        first += s[i]
    elif len(s) % 2 == 1 and i == mid:
        middle = s[i]
    else:
        second += s[i]
print("First Half:", first)
if middle:
    print("Middle:", middle)
print("Second Half:", second)
```

## Q48. Compare Two Halves
```python
s = input()
mid = len(s)//2
same = True
for i in range(mid):
    if s[i] != s[i+mid]:
        same = False
if same:
    print("Equal Halves")
else:
    print("Different Halves")
```

## Q49. Mirror the String
```python
s = input()
same = True
for i in range(len(s)//2):
    if s[i] != s[len(s)-1-i]:
        same = False
if same:
    print("Symmetric")
else:
    print("Not Symmetric")
```

## Q50. Alternate Character Extraction
```python
s = input()
result = ""
for i in range(0, len(s), 2):
    result += s[i]
print(result)
```

## Q51. Count Even and Odd Indexes
```python
s = input()
even = 0
odd = 0
for i in range(len(s)):
    if i % 2 == 0:
        even += 1
    else:
        odd += 1
print("Even Index =", even, "Odd Index =", odd)
```

## Q52. Swap Adjacent Characters
```python
s = input()
result = ""
for i in range(0, len(s), 2):
    result += s[i+1] + s[i]
print(result)
```

## Q53. Second Largest Distinct Digit
```python
n = int(input())
largest = -1
second = -1
for i in range(100):
    if n > 0:
        d = n % 10
        if d > largest:
            second = largest
            largest = d
        elif d < largest and d > second:
            second = d
        n //= 10
print(second)
```

## Q54. Longest Consecutive Equal Character Run
```python
s = input()
current = 0
best = 0
previous = ""
for ch in s:
    if ch == previous:
        current += 1
    else:
        current = 1
    if current > best:
        best = current
    previous = ch
print(best)
```

## Q55. Character Frequency Percentage
```python
s, target = input().replace(",", " ").split()
count = 0
for ch in s:
    if ch == target:
        count += 1
print("Count =", count, "Frequency =", round(count/len(s)*100, 2), "%")
```

## Q56. Running Digit Sum
```python
n = int(input())
total = 0
for i in range(100):
    if n > 0:
        total += n % 10
        print(total)
        n //= 10
```

## Q57. Number with Most Even Digits
```python
n = int(input())
even = 0
odd = 0
for i in range(100):
    if n > 0:
        if (n % 10) % 2 == 0:
            even += 1
        else:
            odd += 1
        n //= 10
if even > odd:
    print("More Even Digits")
elif odd > even:
    print("More Odd Digits")
else:
    print("Equal")
```

## Q58. Alternating Digit Sum
```python
n = int(input())
total = 0
for i in range(100):
    if n > 0:
        d = n % 10
        if i % 2 == 0:
            total += d
        else:
            total -= d
        n //= 10
print(total)
```

## Q59. Accumulator Trap
Output:
```text
2
6
12
20
30
```

## Q60. Condition Inside Loop
Output:
```text
5
```
There are five even numbers from 1 to 10.

## Q61. Debug the Accumulator
Mistake: `sum = i` replaces the previous total.

```python
total = 0
for i in range(1, 6):
    total = total + i
print(total)
```
Output: `15`

## Q62. Daily Expense Analyzer
```python
n = int(input())
values = iter(map(int, input().split()))
total = 0
highest = 0
lowest = 0
for i in range(n):
    x = next(values)
    total += x
    if i == 0 or x > highest:
        highest = x
    if i == 0 or x < lowest:
        lowest = x
print("Total:", total)
print("Highest:", highest)
print("Lowest:", lowest)
```

## Q63. Student Marks Analyzer
```python
n = int(input())
values = iter(map(int, input().split()))
total = 0
highest = 0
lowest = 0
for i in range(n):
    x = next(values)
    total += x
    if i == 0 or x > highest:
        highest = x
    if i == 0 or x < lowest:
        lowest = x
print("Total:", total)
print("Average:", total/n)
print("Highest:", highest)
print("Lowest:", lowest)
```

## Q64. Attendance Analyzer
```python
n = int(input())
values = iter(input().split())
present = 0
absent = 0
for i in range(n):
    x = next(values)
    if x.upper() == "P":
        present += 1
    else:
        absent += 1
print("Present:", present)
print("Absent:", absent)
print("Attendance:", round(present/n*100, 2), "%")
```

## Q65. Electricity Usage Analyzer
```python
n = int(input())
values = iter(map(int, input().split()))
total = 0
days = 0
for i in range(n):
    x = next(values)
    total += x
    if x > 10:
        days += 1
print("Total Units:", total)
print("Days Above 10:", days)
```

## Q66. Shopping Bill Analyzer
```python
n = int(input())
values = iter(map(int, input().split()))
total = 0
count = 0
for i in range(n):
    x = next(values)
    total += x
    if x > 1000:
        count += 1
print("Total Bill:", total)
print("Products Above 1000:", count)
```

## Q67. Login Attempt Analyzer
```python
n = int(input())
values = iter(input().split())
success = 0
failed = 0
for i in range(n):
    x = next(values)
    if x.lower() == "success":
        success += 1
    else:
        failed += 1
print("Successful:", success)
print("Failed:", failed)
print("Success Rate:", success/n*100, "%")
```

## Q68. Number Profile
```python
n = int(input())
digits = 0
total = 0
largest = 0
smallest = 9
even = 0
odd = 0
for i in range(100):
    if n > 0:
        d = n % 10
        digits += 1
        total += d
        if d > largest:
            largest = d
        if d < smallest:
            smallest = d
        if d % 2 == 0:
            even += 1
        else:
            odd += 1
        n //= 10
print("Digits:", digits)
print("Sum:", total)
print("Largest:", largest)
print("Smallest:", smallest)
print("Even Digits:", even)
print("Odd Digits:", odd)
```

## Q69. String Balance Challenge
```python
s = input()
vowels = 0
consonants = 0
upper = 0
lower = 0
even_index = 0
for i, ch in enumerate(s):
    if i % 2 == 0:
        even_index += 1
    if ch != " ":
        if ch.lower() in "aeiou":
            vowels += 1
        elif ch.isalpha():
            consonants += 1
        if ch.isupper():
            upper += 1
        elif ch.islower():
            lower += 1
print("Total Characters:", len(s))
print("Vowels:", vowels)
print("Consonants:", consonants)
print("Uppercase:", upper)
print("Lowercase:", lower)
print("Even Index Characters:", even_index)
```
