# Assignment 5 — Single for Loop

# Q1. Predict the Loop Values
for i in range(2,15,3): print(i)
# Output: 2 5 8 11 14

# Q2. Reverse range()
for i in range(15,2,-3): print(i)
# Output: 15 12 9 6 3

# Q3. How Many Iterations?
for i in range(4,31,5): print(i)
# Output: 4 9 14 19 24 29 (6 iterations)

# Q4. Correct the Boundary
for i in range(3,19,3): print(i)
# Output: 3 6 9 12 15 18

# Q5. Number and Distance from 20
for i in range(5,11): print(i,20-i)
# Output: 5 15; 6 14; 7 13; 8 12; 9 11; 10 10

# Q6. Number, Square and Cube
for i in range(1,7): print(i,i**2,i**3)
# Output: 1 1 1; 2 4 8; 3 9 27; 4 16 64; 5 25 125; 6 36 216

# Q7. Sum of Numbers in a Range
a,b=map(int,input().split()); s=0
for i in range(a,b+1): s+=i
print(s)
# Input: 5 10 | Output: 45

# Q8. Count Multiples of 3
n=int(input()); c=0
for i in range(1,n+1):
    if i%3==0: c+=1
print(c)
# Input: 10 | Output: 3

# Q9. Sum of Multiples of 4
n=int(input()); s=0
for i in range(1,n+1):
    if i%4==0: s+=i
print(s)
# Input: 20 | Output: 60

# Q10. Count Numbers Divisible by 3 and 5
n=int(input()); c=0
for i in range(1,n+1):
    if i%15==0: c+=1
print(c)
# Input: 50 | Output: 3

# Q11. Sum Except Multiples of 3
n=int(input()); s=0
for i in range(1,n+1):
    if i%3!=0: s+=i
print(s)
# Input: 10 | Output: 37

# Q12. Count Even and Odd
n=int(input()); e=o=0
for i in range(1,n+1):
    if i%2==0: e+=1
    else: o+=1
print("Even =",e,"Odd =",o)
# Input: 10 | Output: Even = 5, Odd = 5

# Q13. Running Sum
n=int(input()); s=0
for i in range(1,n+1): s+=i; print(s)
# Input: 5 | Output: 1 3 6 10 15

# Q14. Running Product
n=int(input()); p=1
for i in range(1,n+1): p*=i; print(p)
# Input: 5 | Output: 1 2 6 24 120

# Q15. Factorial
n=int(input()); f=1
for i in range(1,n+1): f*=i
print(f)
# Input: 5 | Output: 120

# Q16. Factorials from 1 to N
n=int(input()); f=1
for i in range(1,n+1): f*=i; print(str(i)+"! =",f)
# Input: 5 | Output: 1!=1; 2!=2; 3!=6; 4!=24; 5!=120

# Q17. Product of Even Numbers
n=int(input()); p=1
for i in range(2,n+1,2): p*=i
print(p)
# Input: 10 | Output: 3840

# Q18. Product of Odd Numbers
n=int(input()); p=1
for i in range(1,n+1,2): p*=i
print(p)
# Input: 7 | Output: 105

# Q19. Even Double Factorial
n=int(input()); p=1
for i in range(2,n+1,2): p*=i
print(p)
# Input: 8 | Output: 384

# Q20. Sum of Squares
n=int(input()); s=0
for i in range(1,n+1): s+=i*i
print(s)
# Input: 5 | Output: 55

# Q21. Sum of Cubes
n=int(input()); s=0
for i in range(1,n+1): s+=i**3
print(s)
# Input: 4 | Output: 100

# Q22. Factorial-Based Sum
n=int(input()); f=s=1
for i in range(1,n+1): f*=i; s+=f
print(s-1)
# Input: 4 | Output: 33

# Q23. Count Digits Without String Conversion
n=int(input()); c=0
for i in range(100):
    if n>0: c+=1; n//=10
print(c)
# Input: 58321 | Output: 5

# Q24. Sum of Digits
n=int(input()); s=0
for i in range(100):
    if n>0: s+=n%10; n//=10
print(s)
# Input: 58321 | Output: 19

# Q25. Product of Digits
n=int(input()); p=1
for i in range(100):
    if n>0: p*=n%10; n//=10
print(p)
# Input: 234 | Output: 24

# Q26. Count Even Digits
n=int(input()); c=0
for i in range(100):
    if n>0:
        if n%10%2==0: c+=1
        n//=10
print(c)
# Input: 58321 | Output: 2

# Q27. Sum of Even Digits
n=int(input()); s=0
for i in range(100):
    if n>0:
        d=n%10
        if d%2==0: s+=d
        n//=10
print(s)
# Input: 58321 | Output: 10

# Q28. Largest Digit Without max()
n=int(input()); big=0
for i in range(100):
    if n>0:
        d=n%10
        if d>big: big=d
        n//=10
print(big)
# Input: 58321 | Output: 8

# Q29. Smallest Digit Without min()
n=int(input()); small=9
for i in range(100):
    if n>0:
        d=n%10
        if d<small: small=d
        n//=10
print(small)
# Input: 58321 | Output: 1

# Q30. Reverse a Number
n=int(input()); rev=0
for i in range(100):
    if n>0: rev=rev*10+n%10; n//=10
print(rev)
# Input: 58321 | Output: 12385

# Q31. Palindrome Number
n=int(input()); old=n; rev=0
for i in range(100):
    if n>0: rev=rev*10+n%10; n//=10
print("Palindrome" if old==rev else "Not Palindrome")
# Input: 1221 | Output: Palindrome

# Q32. Count a Specific Digit
n,t=map(int,input().replace(","," ").split()); c=0
for i in range(100):
    if n>0:
        if n%10==t: c+=1
        n//=10
print(c)
# Input: 1223342, 2 | Output: 3

# Q33. First Digit
n=int(input())
for i in range(100):
    if n>=10: n//=10
print(n)
# Input: 58321 | Output: 5

# Q34. Difference Between Largest and Smallest
n=int(input()); big=0; small=9
for i in range(100):
    if n>0:
        d=n%10
        if d>big: big=d
        if d<small: small=d
        n//=10
print(big-small)
# Input: 58321 | Output: 7

# Q35. Digit Position
n=int(input()); pos=1
for i in range(100):
    if n>0: print(n%10,pos); n//=10; pos+=1
# Input: 58321 | Output: 1 1; 2 2; 3 3; 8 4; 5 5

# Q36. Armstrong Number
n=int(input()); old=n; s=0
for i in range(3): s+=(n%10)**3; n//=10
print("Armstrong Number" if s==old else "Not Armstrong Number")
# Input: 153 | Output: Armstrong Number

# Q37. Characters with Index
s=input()
for i in range(len(s)): print(i,s[i])
# Input: Python | Output: 0 P; 1 y; 2 t; 3 h; 4 o; 5 n

# Q38. Count Characters Without len()
s=input(); c=0
for ch in s: c+=1
print(c)
# Input: Python | Output: 6

# Q39. Count Vowels and Consonants
s=input(); v=c=0
for ch in s.lower():
    if ch in "aeiou": v+=1
    elif ch.isalpha(): c+=1
print("Vowels =",v,"Consonants =",c)
# Input: Python | Output: Vowels = 1, Consonants = 5

# Q40. Character Frequency
s,t=input().replace(","," ").split(); c=0
for ch in s:
    if ch==t: c+=1
print(c)
# Input: programming, g | Output: 2

# Q41. First Occurrence Position
s,t=input().replace(","," ").split(); pos=-1
for i in range(len(s)):
    if s[i]==t and pos==-1: pos=i
print("Not Found" if pos==-1 else pos)
# Input: programming, g | Output: 3

# Q42. Count Uppercase and Lowercase
s=input(); u=l=0
for ch in s:
    if ch.isupper(): u+=1
    elif ch.islower(): l+=1
print("Uppercase =",u,"Lowercase =",l)
# Input: PyThOn | Output: Uppercase = 3, Lowercase = 3

# Q43. Character Code Analyzer
s=input()
for ch in s: print(ch,ord(ch))
# Input: ABC | Output: A 65; B 66; C 67

# Q44. String Without Vowels
s=input(); out=""
for ch in s:
    if ch.lower() not in "aeiou": out+=ch
print(out)
# Input: education | Output: dctn

# Q45. Middle Character
s=input(); print(s[len(s)//2])
# Input: Python | Output: h

# Q46. First Half and Second Half
s=input(); m=len(s)//2
print("First Half:",s[:m]); print("Second Half:",s[m:])
# Input: PythonCode | Output: First Half: Pytho; Second Half: nCode

# Q47. Split String Without Slicing
s=input(); m=len(s)//2; a=b=c=""
for i in range(len(s)):
    if i<m: a+=s[i]
    elif len(s)%2 and i==m: b=s[i]
    else: c+=s[i]
print("First Half:",a)
if b: print("Middle:",b)
print("Second Half:",c)
# Input: PROGRAM | Output: First Half: PRO; Middle: G; Second Half: RAM

# Q48. Compare Two Halves
s=input(); m=len(s)//2; same=True
for i in range(m):
    if s[i]!=s[i+m]: same=False
print("Equal Halves" if same else "Different Halves")
# Input: ABCABC | Output: Equal Halves

# Q49. Mirror the String
s=input(); same=True
for i in range(len(s)//2):
    if s[i]!=s[len(s)-1-i]: same=False
print("Symmetric" if same else "Not Symmetric")
# Input: ABCCBA | Output: Symmetric

# Q50. Alternate Character Extraction
s=input(); out=""
for i in range(0,len(s),2): out+=s[i]
print(out)
# Input: ABCDEFGH | Output: ACEG

# Q51. Count Even and Odd Indexes
s=input(); e=o=0
for i in range(len(s)):
    if i%2==0: e+=1
    else: o+=1
print("Even Index =",e,"Odd Index =",o)
# Input: Python | Output: Even Index = 3, Odd Index = 3

# Q52. Swap Adjacent Characters
s=input(); out=""
for i in range(0,len(s),2): out+=s[i+1]+s[i]
print(out)
# Input: ABCD | Output: BADC

# Q53. Second Largest Distinct Digit
n=int(input()); big=second=-1
for i in range(100):
    if n>0:
        d=n%10
        if d>big: second=big; big=d
        elif d<big and d>second: second=d
        n//=10
print(second)
# Input: 58321 | Output: 5

# Q54. Longest Consecutive Equal Character Run
s=input(); prev=""; cur=best=0
for ch in s:
    if ch==prev: cur+=1
    else: cur=1
    if cur>best: best=cur
    prev=ch
print(best)
# Input: aaabbccccd | Output: 4

# Q55. Character Frequency Percentage
s,t=input().replace(","," ").split(); c=0
for ch in s:
    if ch==t: c+=1
print("Count =",c,"Frequency =",str(round(c/len(s)*100,2))+"%")
# Input: banana, a | Output: Count = 3, Frequency = 50.0%

# Q56. Running Digit Sum
n=int(input()); s=0
for i in range(100):
    if n>0: s+=n%10; print(s); n//=10
# Input: 58321 | Output: 1; 3; 6; 14; 19

# Q57. Number with Most Even Digits
n=int(input()); e=o=0
for i in range(100):
    if n>0:
        if (n%10)%2==0: e+=1
        else: o+=1
        n//=10
print("More Even Digits" if e>o else "More Odd Digits" if o>e else "Equal")
# Input: 24681 | Output: More Even Digits

# Q58. Alternating Digit Sum
n=int(input()); s=0
for i in range(100):
    if n>0:
        d=n%10
        if i%2==0: s+=d
        else: s-=d
        n//=10
print(s)
# Input: 12345 | Output: 3

# Q59. Accumulator Trap
# Output: 2; 6; 12; 20; 30

# Q60. Condition Inside Loop
# Output: 5
# There are five even numbers from 1 to 10.

# Q61. Debug the Accumulator
total=0
for i in range(1,6): total+=i
print(total)
# Mistake: sum=i replaces the previous total.
# Output: 15

# Q62. Daily Expense Analyzer
n=int(input()); vals=iter(map(int,input().split())); total=0
high=low=0
for i in range(n):
    x=next(vals); total+=x
    if i==0 or x>high: high=x
    if i==0 or x<low: low=x
print("Total:",total); print("Highest:",high); print("Lowest:",low)
# Input: 5 / 250 180 400 120 300
# Output: Total: 1250; Highest: 400; Lowest: 120

# Q63. Student Marks Analyzer
n=int(input()); vals=iter(map(int,input().split())); total=0
high=low=0
for i in range(n):
    x=next(vals); total+=x
    if i==0 or x>high: high=x
    if i==0 or x<low: low=x
print("Total:",total); print("Average:",total/n); print("Highest:",high); print("Lowest:",low)
# Input: 5 / 78 65 92 81 74
# Output: Total: 390; Average: 78.0; Highest: 92; Lowest: 65

# Q64. Attendance Analyzer
n=int(input()); vals=iter(input().split()); p=a=0
for i in range(n):
    if next(vals).upper()=="P": p+=1
    else: a+=1
print("Present:",p); print("Absent:",a); print("Attendance:",str(round(p/n*100,2))+"%")
# Input: 6 / P P A P A P
# Output: Present: 4; Absent: 2; Attendance: 66.67%

# Q65. Electricity Usage Analyzer
n=int(input()); vals=iter(map(int,input().split())); total=days=0
for i in range(n):
    x=next(vals); total+=x
    if x>10: days+=1
print("Total Units:",total); print("Days Above 10:",days)
# Input: 5 / 8 12 15 7 13
# Output: Total Units: 55; Days Above 10: 3

# Q66. Shopping Bill Analyzer
n=int(input()); vals=iter(map(int,input().split())); total=c=0
for i in range(n):
    x=next(vals); total+=x
    if x>1000: c+=1
print("Total Bill:",total); print("Products Above 1000:",c)
# Input: 5 / 450 1200 800 2500 600
# Output: Total Bill: 5550; Products Above 1000: 2

# Q67. Login Attempt Analyzer
n=int(input()); vals=iter(input().split()); success=failed=0
for i in range(n):
    if next(vals).lower()=="success": success+=1
    else: failed+=1
print("Successful:",success); print("Failed:",failed); print("Success Rate:",str(success/n*100)+"%")
# Input: 5 / success failed success failed success
# Output: Successful: 3; Failed: 2; Success Rate: 60.0%

# Q68. Number Profile
n=int(input()); digits=total=even=odd=0; big=0; small=9
for i in range(100):
    if n>0:
        d=n%10; digits+=1; total+=d
        if d>big: big=d
        if d<small: small=d
        if d%2==0: even+=1
        else: odd+=1
        n//=10
print("Digits:",digits); print("Sum:",total); print("Largest:",big); print("Smallest:",small); print("Even Digits:",even); print("Odd Digits:",odd)
# Input: 58321
# Output: Digits: 5; Sum: 19; Largest: 8; Smallest: 1; Even Digits: 2; Odd Digits: 3

# Q69. String Balance Challenge
s=input(); v=c=u=l=e=0
for i,ch in enumerate(s):
    if i%2==0: e+=1
    if ch!=" ":
        if ch.lower() in "aeiou": v+=1
        elif ch.isalpha(): c+=1
        if ch.isupper(): u+=1
        elif ch.islower(): l+=1
print("Total Characters:",len(s)); print("Vowels:",v); print("Consonants:",c); print("Uppercase:",u); print("Lowercase:",l); print("Even Index Characters:",e)
# Input: Hello World
# Output: Total Characters: 11; Vowels: 3; Consonants: 7; Uppercase: 2; Lowercase: 8; Even Index Characters: 6
