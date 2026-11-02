# Assignment 6 – Nested for Loop
## Part 1: Pattern Programs (Q1–Q65)

### Level 1 – Basic Patterns

**Q1. Solid Square**
``` 
n = int(input("Enter size: "))
for i in range(n):
    for j in range(n):
        print("*", end="")
    print()
```

**Q2. Solid Rectangle**
```
r = int(input("Enter rows: "))
c = int(input("Enter columns: "))
for i in range(r):
    for j in range(c):
        print("*", end="")
    print()
```

**Q3. Increasing Star Triangle**
```
n = int(input("Enter size: "))
for i in range(1, n + 1):
    for j in range(i):
        print("*", end="")
    print()
```

**Q4. Increasing Number Triangle**
```
n = int(input("Enter size: "))
for i in range(1, n + 1):
    for j in range(1, i + 1):
        print(j, end="")
    print()
```

**Q5. Repeated Number Triangle**
```
n = int(input("Enter size: "))
for i in range(1, n + 1):
    for j in range(i):
        print(i, end="")
    print()
```

**Q6. Repeated Alphabet Triangle**
```
n = int(input("Enter size: "))
for i in range(n):
    for j in range(i + 1):
        print(chr(65 + i), end="")
    print()
```

**Q7. Alphabet Triangle**
```
n = int(input("Enter size: "))
for i in range(1, n + 1):
    for j in range(i):
        print(chr(65 + j), end="")
    print()
```

**Q8. Continuous Number Triangle**
```
n = int(input("Enter size: "))
num = 1
for i in range(1, n + 1):
    for j in range(i):
        print(num, end=" ")
        num += 1
    print()
```

**Q9. Alternating 0–1 Triangle**
```
n = int(input("Enter size: "))
for i in range(1, n + 1):
    for j in range(i):
        print((i + j + 1) % 2, end=" ")
    print()
```

**Q10. Decreasing Star Triangle**
```
n = int(input("Enter size: "))
for i in range(n, 0, -1):
    for j in range(i):
        print("*", end="")
    print()
```

**Q11. Decreasing Number Triangle**
```
n = int(input("Enter size: "))
for i in range(n, 0, -1):
    for j in range(1, i + 1):
        print(j, end="")
    print()
```

**Q12. Decreasing Alphabet Triangle**
```
n = int(input("Enter size: "))
for i in range(n, 0, -1):
    for j in range(i):
        print(chr(65 + j), end="")
    print()
```

### Level 2 – Spaces and Alignment

**Q13. Right-Aligned Half Pyramid**
```
n = int(input("Enter size: "))
for i in range(1, n + 1):
    for j in range(n - i):
        print(" ", end="")
    for j in range(i):
        print("*", end="")
    print()
```

**Q14. Inverted Right-Aligned Half Pyramid**
```
n = int(input("Enter size: "))
for i in range(n, 0, -1):
    for j in range(n - i):
        print(" ", end="")
    for j in range(i):
        print("*", end="")
    print()
```

**Q15. Star Pyramid**
```
n = int(input("Enter size: "))
for i in range(1, n + 1):
    for j in range(n - i):
        print(" ", end="")
    for j in range(2 * i - 1):
        print("*", end="")
    print()
```

**Q16. Inverted Star Pyramid**
```
n = int(input("Enter size: "))
for i in range(n, 0, -1):
    for j in range(n - i):
        print(" ", end="")
    for j in range(2 * i - 1):
        print("*", end="")
    print()
```

**Q17. Solid Diamond**
```
n = int(input("Enter size: "))
for i in range(1, n + 1):
    for j in range(n - i):
        print(" ", end="")
    for j in range(2 * i - 1):
        print("*", end="")
    print()
for i in range(n - 1, 0, -1):
    for j in range(n - i):
        print(" ", end="")
    for j in range(2 * i - 1):
        print("*", end="")
    print()
```

**Q18. Rhombus**
```
n = int(input("Enter size: "))
for i in range(n):
    for j in range(n - i - 1):
        print(" ", end="")
    for j in range(n):
        print("*", end="")
    print()
```

**Q19. Mirrored Number Pattern**
```
n = int(input("Enter size: "))
for i in range(1, n + 1):
    for j in range(1, i + 1):
        print(j, end="")
    for j in range(2 * (n - i)):
        print(" ", end="")
    for j in range(i, 0, -1):
        print(j, end="")
    print()
```

**Q20. Centered Number Pyramid**
```
n = int(input("Enter size: "))
for i in range(1, n + 1):
    for j in range(n - i):
        print(" ", end="")
    for j in range(1, i + 1):
        print(j, end=" ")
    print()
```

**Q21. Palindromic Number Pyramid**
```
n = int(input("Enter size: "))
for i in range(1, n + 1):
    for j in range(n - i):
        print(" ", end="")
    for j in range(1, i + 1):
        print(j, end="")
    for j in range(i - 1, 0, -1):
        print(j, end="")
    print()
```

**Q22. Alphabet Palindrome Pyramid**
```
n = int(input("Enter size: "))
for i in range(1, n + 1):
    for j in range(n - i):
        print(" ", end="")
    for j in range(i):
        print(chr(65 + j), end="")
    for j in range(i - 2, -1, -1):
        print(chr(65 + j), end="")
    print()
```

**Q23. Reverse-Starting Alphabet Triangle**
```
n = int(input("Enter size: "))
for i in range(n):
    for j in range(n - i - 1, n):
        print(chr(65 + j), end=" ")
    print()
```

### Level 3 – Mixed Logic and Repeated Sequences

**Q24. Increasing and Decreasing Star Triangle**
```
n = int(input("Enter size: "))
for i in range(1, n + 1):
    for j in range(i):
        print("*", end="")
    print()
for i in range(n - 1, 0, -1):
    for j in range(i):
        print("*", end="")
    print()
```

**Q25. Number Hourglass**
```
n = int(input("Enter size: "))
for i in range(n, 0, -1):
    for j in range(1, i + 1):
        print(j, end="")
    print()
for i in range(2, n + 1):
    for j in range(1, i + 1):
        print(j, end="")
    print()
```

**Q26. Alphabet Hourglass**
```
n = int(input("Enter size: "))
for i in range(n, 0, -1):
    for j in range(i):
        print(chr(65 + j), end="")
    print()
for i in range(2, n + 1):
    for j in range(i):
        print(chr(65 + j), end="")
    print()
```

**Q27. Alternating Star and Hash Grid**
```
n = int(input("Enter size: "))
for i in range(n):
    for j in range(n):
        if (i + j) % 2 == 0:
            print("*", end="")
        else:
            print("#", end="")
    print()
```

**Q28. Binary Checkerboard**
```
n = int(input("Enter size: "))
for i in range(n):
    for j in range(n):
        print(1 - (i + j) % 2, end="")
    print()
```

**Q29. Multiplication Grid**
```
n = int(input("Enter size: "))
for i in range(1, n + 1):
    for j in range(1, n + 1):
        print(i * j, end=" ")
    print()
```

**Q30. Alternating-Direction Rows**
```
n = int(input("Enter size: "))
for i in range(1, n + 1):
    if i % 2 == 0:
        for j in range(i, 0, -1):
            print(j, end="")
    else:
        for j in range(1, i + 1):
            print(j, end="")
    print()
```

**Q31. Number Diamond**
```
n = int(input("Enter size: "))
for i in range(1, n + 1):
    for j in range(n - i):
        print(" ", end="")
    for j in range(1, i + 1):
        print(j, end="")
    for j in range(i - 1, 0, -1):
        print(j, end="")
    print()
for i in range(n - 1, 0, -1):
    for j in range(n - i):
        print(" ", end="")
    for j in range(1, i + 1):
        print(j, end="")
    for j in range(i - 1, 0, -1):
        print(j, end="")
    print()
```

**Q32. Concentric Number Square**
```
n = int(input("Enter size: "))
size = 2 * n - 1
for i in range(size):
    for j in range(size):
        value = n - min(i, j, size - 1 - i, size - 1 - j)
        print(value, end=" ")
    print()
```

### Level 4 – Hollow Patterns and Conditions

**Q33. Hollow Square**
```
n = int(input("Enter size: "))
for i in range(n):
    for j in range(n):
        if i == 0 or i == n - 1 or j == 0 or j == n - 1:
            print("*", end="")
        else:
            print(" ", end="")
    print()
```

**Q34. Hollow Rectangle**
```
r = int(input("Enter rows: "))
c = int(input("Enter columns: "))
for i in range(r):
    for j in range(c):
        if i == 0 or i == r - 1 or j == 0 or j == c - 1:
            print("*", end="")
        else:
            print(" ", end="")
    print()
```

**Q35. Hollow Number Square**
```
n = int(input("Enter size: "))
for i in range(n):
    for j in range(n):
        if i == 0 or i == n - 1 or j == 0 or j == n - 1:
            print("1", end="")
        else:
            print("0", end="")
    print()
```

**Q36. Hollow Right-Angled Triangle**
```
n = int(input("Enter size: "))
for i in range(1, n + 1):
    for j in range(i):
        if j == 0 or j == i - 1 or i == n:
            print("*", end="")
        else:
            print(" ", end="")
    print()
```

**Q37. Hollow Inverted Triangle**
```
n = int(input("Enter size: "))
for i in range(n, 0, -1):
    for j in range(i):
        if j == 0 or j == i - 1 or i == n:
            print("*", end="")
        else:
            print(" ", end="")
    print()
```

**Q38. Hollow Pyramid**
```
n = int(input("Enter size: "))
for i in range(1, n + 1):
    for j in range(n - i):
        print(" ", end="")
    for j in range(2 * i - 1):
        if i == n or j == 0 or j == 2 * i - 2:
            print("*", end="")
        else:
            print(" ", end="")
    print()
```

**Q39. Hollow Diamond**
```
n = int(input("Enter size: "))
for i in range(1, n + 1):
    for j in range(n - i):
        print(" ", end="")
    for j in range(2 * i - 1):
        if j == 0 or j == 2 * i - 2:
            print("*", end="")
        else:
            print(" ", end="")
    print()
for i in range(n - 1, 0, -1):
    for j in range(n - i):
        print(" ", end="")
    for j in range(2 * i - 1):
        if j == 0 or j == 2 * i - 2:
            print("*", end="")
        else:
            print(" ", end="")
    print()
```

**Q40. X Pattern**
```
n = int(input("Enter odd size: "))
for i in range(n):
    for j in range(n):
        if j == i or j == n - 1 - i:
            print("*", end="")
        else:
            print(" ", end="")
    print()
```

**Q41. Cross Pattern**
```
n = int(input("Enter odd size: "))
for i in range(n):
    for j in range(n):
        if j == i or j == n - 1 - i or i == n // 2:
            print("*", end="")
        else:
            print(" ", end="")
    print()
```

**Q42. Star Cross with Four Arms**
```
n = int(input("Enter odd size: "))
for i in range(n):
    for j in range(n):
        if j == i or j == n - 1 - i:
            print("*", end="")
        else:
            print(" ", end="")
    print()
```

### Level 5 – Advanced Shapes and Challenges

**Q43. Butterfly Pattern**
```
n = int(input("Enter size: "))
for i in range(1, n + 1):
    for j in range(i):
        print("*", end="")
    for j in range(2 * (n - i)):
        print(" ", end="")
    for j in range(i):
        print("*", end="")
    print()
for i in range(n - 1, 0, -1):
    for j in range(i):
        print("*", end="")
    for j in range(2 * (n - i)):
        print(" ", end="")
    for j in range(i):
        print("*", end="")
    print()
```

**Q44. Hollow Hourglass**
```
n = int(input("Enter size: "))
for i in range(n, 0, -1):
    for j in range(n - i):
        print(" ", end="")
    for j in range(2 * i - 1):
        if i == n or j == 0 or j == 2 * i - 2:
            print("*", end="")
        else:
            print(" ", end="")
    print()
for i in range(2, n + 1):
    for j in range(n - i):
        print(" ", end="")
    for j in range(2 * i - 1):
        if i == n or j == 0 or j == 2 * i - 2:
            print("*", end="")
        else:
            print(" ", end="")
    print()
```

**Q45. Alphabet Diamond**
```
n = int(input("Enter size: "))
for i in range(1, n + 1):
    for j in range(n - i):
        print(" ", end="")
    for j in range(i):
        print(chr(65 + j), end="")
    for j in range(i - 2, -1, -1):
        print(chr(65 + j), end="")
    print()
for i in range(n - 1, 0, -1):
    for j in range(n - i):
        print(" ", end="")
    for j in range(i):
        print(chr(65 + j), end="")
    for j in range(i - 2, -1, -1):
        print(chr(65 + j), end="")
    print()
```

**Q46. Pascal's Triangle**
```
n = int(input("Enter rows: "))
for i in range(n):
    num = 1
    for j in range(n - i - 1):
        print(" ", end="")
    for j in range(i + 1):
        print(num, end=" ")
        num = num * (i - j) // (j + 1)
    print()
```

**Q47. Heart Pattern**
```
n = int(input("Enter size (at least 5): "))
for i in range(n // 2, n, 2):
    for j in range(n - i):
        print(" ", end="")
    for j in range(i):
        print("*", end="")
    for j in range(n - i):
        print(" ", end="")
    for j in range(i):
        print("*", end="")
    print()
for i in range(n, 0, -1):
    for j in range(n - i):
        print(" ", end="")
    for j in range(2 * i - 1):
        print("*", end="")
    print()
```

**Q48. Hollow Heart**
```
n = int(input("Enter size (at least 5): "))
for i in range(n // 2, n, 2):
    for j in range(n - i):
        print(" ", end="")
    for j in range(i):
        if j == 0 or j == i - 1:
            print("*", end="")
        else:
            print(" ", end="")
    for j in range(n - i):
        print(" ", end="")
    for j in range(i):
        if j == 0 or j == i - 1:
            print("*", end="")
        else:
            print(" ", end="")
    print()
for i in range(n, 0, -1):
    for j in range(n - i):
        print(" ", end="")
    for j in range(2 * i - 1):
        if j == 0 or j == 2 * i - 2:
            print("*", end="")
        else:
            print(" ", end="")
    print()
```

**Q49. Star-and-Space Center Pattern**
```
n = int(input("Enter odd size: "))
for i in range(n):
    for j in range(n):
        if j == i or j == n - 1 - i or i == n // 2:
            print("*", end="")
        else:
            print(" ", end="")
    print()
```

**Q50. Custom Symbol Square**
```
n = int(input("Enter size: "))
symbol = input("Enter symbol: ")
for i in range(n):
    for j in range(n):
        print(symbol, end="")
    print()
```

**Q51. User-Sized Hollow Rectangle**
```
r = int(input("Enter rows: "))
c = int(input("Enter columns: "))
for i in range(r):
    for j in range(c):
        if i == 0 or i == r - 1 or j == 0 or j == c - 1:
            print("*", end="")
        else:
            print(" ", end="")
    print()
```

**Q52. Create Your Own Pattern – Example**
```
n = int(input("Enter size: "))
for i in range(1, n + 1):
    for j in range(i):
        print("#", end="")
    print()
```

### Level 6 – Additional Patterns

**Q53. Number Increasing Reverse Pyramid**
```
n = int(input("Enter size: "))
for i in range(n, 0, -1):
    for j in range(1, i + 1):
        print(j, end=" ")
    print()
```

**Q54. Square Fill Pattern**
```
n = int(input("Enter size: "))
for i in range(n):
    for j in range(n):
        print("*", end=" ")
    print()
```

**Q55. Left Half Pyramid**
```
n = int(input("Enter size: "))
for i in range(1, n + 1):
    for j in range(n - i):
        print(" ", end="")
    for j in range(2 * i - 1):
        print("*", end="")
    print()
```

**Q56. Reverse Right Half Pyramid**
```
n = int(input("Enter size: "))
for i in range(n, 0, -1):
    for j in range(i):
        print("*", end="")
    print()
```

**Q57. Left Half Pyramid – Increasing**
```
n = int(input("Enter size: "))
for i in range(1, n + 1):
    for j in range(i):
        print("*", end="")
    print()
```

**Q58. Reverse Left Half Pyramid**
```
n = int(input("Enter size: "))
for i in range(n, 0, -1):
    for j in range(n - i):
        print(" ", end="")
    for j in range(i):
        print("*", end="")
    print()
```

**Q59. Triangle Star Pattern**
```
n = int(input("Enter size: "))
for i in range(1, n + 1):
    for j in range(n - i):
        print(" ", end="")
    for j in range(i):
        print("*", end="")
    print()
```

**Q60. Mirror-Image Number Triangle**
```
n = int(input("Enter size: "))
for i in range(1, n + 1):
    for j in range(i - 1):
        print(" ", end="")
    for j in range(i, n + 1):
        print(j, end=" ")
    print()
```

**Q61. Hollow Reverse Triangle**
```
n = int(input("Enter size: "))
for i in range(n):
    for j in range(i):
        print(" ", end="")
    for j in range(n - i):
        if j == 0 or j == n - i - 1 or i == 0:
            print("*", end="")
        else:
            print(" ", end="")
    print()
```

**Q62. Hollow Diamond Pyramid**
```
n = int(input("Enter size: "))
for i in range(1, n + 1):
    for j in range(n - i):
        print(" ", end="")
    for j in range(2 * i - 1):
        if j == 0 or j == 2 * i - 2:
            print("*", end="")
        else:
            print(" ", end="")
    print()
for i in range(n - 1, 0, -1):
    for j in range(n - i):
        print(" ", end="")
    for j in range(2 * i - 1):
        if j == 0 or j == 2 * i - 2:
            print("*", end="")
        else:
            print(" ", end="")
    print()
```

**Q63. Hollow Hourglass Pattern**
```
n = int(input("Enter size: "))
for i in range(n, 0, -1):
    for j in range(n - i):
        print(" ", end="")
    for j in range(2 * i - 1):
        if j == 0 or j == 2 * i - 2:
            print("*", end="")
        else:
            print(" ", end="")
    print()
for i in range(2, n + 1):
    for j in range(n - i):
        print(" ", end="")
    for j in range(2 * i - 1):
        if j == 0 or j == 2 * i - 2:
            print("*", end="")
        else:
            print(" ", end="")
    print()
```

**Q64. Right Pascal's Triangle**
```
n = int(input("Enter size: "))
for i in range(1, n + 1):
    for j in range(i):
        print("*", end="")
    print()
for i in range(n - 1, 0, -1):
    for j in range(i):
        print("*", end="")
    print()
```

**Q65. Pattern Size Challenge**

Test the programs above using three different sizes, for example:
```
n = 3
n = 5
n = 7
```
Check that the number of rows, columns, spaces, and symbols changes correctly.
