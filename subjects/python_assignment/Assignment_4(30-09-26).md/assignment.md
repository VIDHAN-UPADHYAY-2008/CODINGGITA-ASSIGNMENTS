# Assignment 4 — Conditional Statements, Nested Conditions & Match-Case

```python
# Q1
n=int(input())
if n>0: print("Positive Number")

# Q2
age=int(input())
if age>=18: print("Eligible to Vote")

# Q3
t=int(input())
if t>40: print("High Temperature")

# Q4
n=int(input())
if n%5==0: print("Divisible by 5")

# Q5
a=int(input())
if a>=1000: print("Free Delivery")

# Q6
c=input()
if c=="A": print("You entered A")

# Q7
p=input()
if len(p)>=8: print("Strong Length")

# Q8
n=int(input())
if 100<=n<=999: print("Three Digit Number")

# Q9
n=int(input())
if n%2==0: print("Even")
else: print("Odd")

# Q10
m=int(input())
if m>=40: print("Pass")
else: print("Fail")

# Q11
age=int(input())
if age>=18: print("Adult")
else: print("Minor")

# Q12
n=int(input())
if n>0: print("Positive")
else: print("Non-Positive")

# Q13
n=int(input())
if n%3==0: print("Divisible by 3")
else: print("Not Divisible by 3")

# Q14
p=input()
if p=="python123": print("Login Successful")
else: print("Invalid Password")

# Q15
u=input()
if u=="admin": print("Welcome Admin")
else: print("Invalid Username")

# Q16
a,b=map(int,input().split())
if a>b: print(a)
elif b>a: print(b)
else: print("Both are Equal")

# Q17
t=int(input())
if t>30: print("Hot")
else: print("Comfortable")

# Q18
a=int(input())
if a>=5000: print("Discount Available")
else: print("No Discount")

# Q19
m=int(input())
if m>=90: print("A")
elif m>=80: print("B")
elif m>=70: print("C")
elif m>=60: print("D")
else: print("F")

# Q20
t=int(input())
if t>=40: print("Very Hot")
elif t>=30: print("Hot")
elif t>=20: print("Warm")
else: print("Cold")

# Q21
s=input()
if s=="red": print("Stop")
elif s=="yellow": print("Wait")
elif s=="green": print("Go")
else: print("Invalid Signal")

# Q22
u=int(input())
if u<=100: print("Low Usage")
elif u<=300: print("Medium Usage")
elif u<=500: print("High Usage")
else: print("Very High Usage")

# Q23
age=int(input())
if age<5: print("Free Ticket")
elif age<=12: print("Child Ticket")
elif age<=59: print("Regular Ticket")
else: print("Senior Ticket")

# Q24
b=float(input())
if b<18.5: print("Underweight")
elif b<25: print("Normal")
elif b<30: print("Overweight")
else: print("Obese")

# Q25
m=int(input())
if m==2: print("28 or 29 Days")
elif m==4 or m==6 or m==9 or m==11: print("30 Days")
elif 1<=m<=12: print("31 Days")
else: print("Invalid Month")

# Q26
a,b=map(float,input().split()); op=input()
if op=="+": print(a+b)
elif op=="-": print(a-b)
elif op=="*": print(a*b)
elif op=="/": print(a/b)
else: print("Invalid Operator")

# Q27
d=int(input())
if d==1: print("Monday")
elif d==2: print("Tuesday")
elif d==3: print("Wednesday")
elif d==4: print("Thursday")
elif d==5: print("Friday")
elif d==6: print("Saturday")
elif d==7: print("Sunday")
else: print("Invalid Day")

# Q28
s=int(input())
if s>=90: print("Excellent")
elif s>=75: print("Very Good")
elif s>=60: print("Good")
elif s>=40: print("Average")
else: print("Needs Improvement")

# Q29
m,a=map(int,input().split())
if m>=60 and a>=75: print("Eligible")
else: print("Not Eligible")

# Q30
m,i=map(int,input().split())
if m>=85 or i<300000: print("Scholarship Available")
else: print("No Scholarship")

# Q31
d=input()
if d=="Saturday" or d=="Sunday": print("Weekend")
else: print("Weekday")

# Q32
u,p=input().split()
if u=="student" and p=="python123": print("Access Granted")
else: print("Access Denied")

# Q33
c=input()
if c=="Ahmedabad" or c=="Gandhinagar": print("Delivery Available")
else: print("Delivery Unavailable")

# Q34
n=int(input())
if 10<=n<=50: print("Inside Range")
else: print("Outside Range")

# Q35
a,o=input().split(); a=int(a)
if a<=50000 and o=="1234": print("Transaction Approved")
else: print("Transaction Declined")

# Q36
u,p=input().split()
if u=="admin":
    if p=="admin123": print("Login Successful")
    else: print("Wrong Password")
else: print("Invalid Username")

# Q37
age,status=input().split(); age=int(age)
if age>=18:
    if status=="pass": print("License Approved")
    else: print("Test Not Passed")
else: print("Age Not Eligible")

# Q38
b,w=map(int,input().split())
if w<=b:
    if w%100==0: print("Withdrawal Successful")
    else: print("Enter Amount in Multiples of 100")
else: print("Insufficient Balance")

# Q39
a,m=map(int,input().split())
if a>=75:
    if m>=40: print("Pass")
    else: print("Fail")
else: print("Not Eligible Due to Attendance")

# Q40
t,b=input().split(); b=int(b)
if t=="savings":
    if b>=1000: print("Minimum Balance Maintained")
    else: print("Minimum Balance Not Maintained")
else: print("Unsupported Account")

# Q41
a,p=input().split(); a=int(a)
if a>=500:
    if p=="card": print("Card Payment Accepted")
    elif p=="upi": print("UPI Payment Accepted")
    else: print("Unsupported Payment Method")
else: print("Minimum Order Amount Not Reached")

# Q42
y,a=map(int,input().split())
if y==2 or y==3 or y==4:
    if a>=75: print("Room Eligible")
    else: print("Attendance Too Low")
else: print("Not Eligible by Year")

# Q43
p,u=input().split(); u=int(u)
if p=="basic":
    if u>100: print("Recommend Upgrade")
    else: print("Basic Plan Is Sufficient")
else: print("Already on Higher Plan")

# Q44
a,b,c=map(int,input().split())
if a==b==c: print("All are Equal")
elif a==b and a>c: print("A and B are Equal and Greatest")
elif a==c and a>b: print("A and C are Equal and Greatest")
elif b==c and b>a: print("B and C are Equal and Greatest")
elif a>b and a>c: print("A is Greatest")
elif b>a and b>c: print("B is Greatest")
else: print("C is Greatest")

# Q45
m,a=map(int,input().split())
if a>=75:
    if m>=90: print("Grade A")
    elif m>=75: print("Grade B")
    elif m>=60: print("Grade C")
    elif m>=40: print("Grade D")
    else: print("Grade F")
else: print("Not Eligible")

# Q46
s,r=map(int,input().split())
if s>=30000:
    if r==5: print("Bonus: 20%")
    elif r==4: print("Bonus: 15%")
    elif r==3: print("Bonus: 10%")
    else: print("Bonus: 5%")
else: print("Not Eligible for Bonus")

# Q47
age,d=map(int,input().split())
if age<5: print("Free")
elif age>=60: print("Senior")
elif d<=10: print("Regular - Short Distance")
else: print("Regular - Long Distance")

# Q48
stock,p=input().split()
if int(stock)>0:
    if p=="paid": print("Order Confirmed")
    elif p=="pending": print("Payment Pending")
    else: print("Invalid Payment Status")
else: print("Out of Stock")

# Q49
age,t=input().split(); age=int(age)
if age<5: print("Free Travel")
elif age>=60: print("Senior Passenger")
elif t=="AC": print("AC Ticket")
elif t=="Sleeper": print("Sleeper Ticket")
else: print("Invalid Ticket Type")

# Q50
n=int(input())
match n:
    case 1: print("Add")
    case 2: print("View")
    case 3: print("Update")
    case 4: print("Delete")
    case _: print("Invalid Choice")

# Q51
n=int(input())
match n:
    case 1: print("Monday")
    case 2: print("Tuesday")
    case 3: print("Wednesday")
    case 4: print("Thursday")
    case 5: print("Friday")
    case 6: print("Saturday")
    case 7: print("Sunday")
    case _: print("Invalid Day")

# Q52
a,b=map(float,input().split()); op=input()
match op:
    case "+": print(a+b)
    case "-": print(a-b)
    case "*": print(a*b)
    case "/": print(a/b)
    case _: print("Invalid Operator")

# Q53
c=input()
match c:
    case "red": print("Stop")
    case "yellow": print("Wait")
    case "green": print("Go")
    case _: print("Invalid Signal")

# Q54
g=input()
match g:
    case "A": print("Excellent Performance")
    case "B": print("Very Good Performance")
    case "C": print("Good Performance")
    case "D": print("Needs Improvement")
    case "F": print("Failed")
    case _: print("Invalid Grade")

# Q55
n=int(input())
match n:
    case 1: print("Check Balance")
    case 2: print("Recharge")
    case 3: print("Data Usage")
    case 4: print("Customer Support")
    case _: print("Invalid Service")

# Q56
m=int(input())
match m:
    case 1: print("January")
    case 2: print("February")
    case 3: print("March")
    case 4: print("April")
    case 5: print("May")
    case 6: print("June")
    case 7: print("July")
    case 8: print("August")
    case 9: print("September")
    case 10: print("October")
    case 11: print("November")
    case 12: print("December")
    case _: print("Invalid Month")

# Q57
e=input()
match e:
    case "py": print("Python File")
    case "txt": print("Text File")
    case "pdf": print("PDF File")
    case "jpg": print("Image File")
    case _: print("Unknown File Type")

# Q58
d=input().split("-")
if d[2]=="CSE": print("CSE Student")
else: print("Non-CSE Student")

# Q59
e=input()
if e.split("@")[1]=="gmail.com": print("Gmail User")
else: print("Other Email Provider")

# Q60
a,b,c=input().split()
u=a+"."+c
if "." in u: print("Valid Username Format")
else: print("Invalid Username Format")

# Q61
n=int(input())
if n<10: print("One Digit")
elif n<100: print("Two Digits")
elif n<1000: print("Three Digits")
else: print("Four or More Digits")

# Q62
p,q=map(float,input().split()); s=p*q
if s>=5000: d=20
elif s>=2000: d=10
else: d=0
f=s-s*d/100
print(f"Subtotal: {s:g}, Discount: {d}%, Final: {f:.2f}")

# Q63
u=int(input())
if u<=100: r=5
elif u<=300: r=7
else: r=10
print(f"Units: {u}\nRate: ₹{r}\nBill: ₹{u*r}")

# Q64
b=10000; c=int(input())
match c:
    case 1: print("Balance:",b)
    case 2:
        a=int(input()); b+=a
        print("Deposit Successful, Balance:",b)
    case 3:
        a=int(input())
        if a<=b:
            b-=a; print("Withdrawal Successful, Balance:",b)
        else: print("Insufficient Balance")
    case 4: print("Exit")
    case _: print("Invalid Choice")

# Q65
c,q=map(int,input().split())
match c:
    case 1: p=250
    case 2: p=150
    case 3: p=200
    case 4: p=120
    case _: p=0
if p==0: print("Invalid Choice")
else:
    t=p*q
    if t>=500: d=t*.1
    else: d=0
    print(f"Total: {t:.0f}, Discount: {d:.2f}, Final: {t-d:.2f}")

# Q66
a,b,c,att=map(int,input().split()); avg=(a+b+c)/3
if att<75: print("Not Eligible")
elif avg>=90: print("Outstanding")
elif avg>=75: print("Very Good")
elif avg>=60: print("Good")
elif avg>=40: print("Pass")
else: print("Fail")

# Q67
d=float(input()); r=input()
match r:
    case "normal": rate=15
    case "premium": rate=25
    case _: rate=0
if rate==0: print("Invalid Ride Type")
else:
    fare=d*rate
    if d>20: fare*=1.1
    print(f"Fare: {fare:.2f}")

# Q68
s,p=map(int,input().split()); c=input()
match c:
    case "general": ok=s>=80 and p>=75
    case "obc": ok=s>=70 and p>=70
    case "sc": ok=s>=60 and p>=60
    case _: ok=False
if ok: print("Admission Eligible")
else: print("Admission Not Eligible")

# Q69
age=int(input())
if age>=18: print("Eligible")
else: print("Not Eligible")

# Q70
m=int(input())
if m>=90: print("A")
elif m>=75: print("B")
elif m>=40: print("Pass")
else: print("Fail")

# Q71
# Output: Pass

# Q72
# 95 → A, 85 → B, 50 → Pass, 30 → Fail

# Q73
# 20,True → Entry Allowed
# 20,False → ID Required
# 16,True → Underage

# Q74
# 1 → Add, 3 → Delete, 5 → Invalid Choice
# case _ = default case

# Q75
# 82,80 → Grade B
# 92,80 → Grade A
# 55,80 → Pass
# 92,60 → Not Eligible
```
