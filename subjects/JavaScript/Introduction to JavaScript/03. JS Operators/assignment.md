# Assignment: JavaScript Operators

## A] Arithmetic Operators

### 1. Addition (+)

**1.** ₹15,000 + ₹12,500 = **₹27,500**

**2.** 18 + 25 = **43 pages**

**3.** 125 + 178 = **303 items**

**4.**

```javascript
let a = "10";
let b = 5;
let result = a + b;
console.log(result);
```

**Answer:** `"105"`
Because `+` joins string and number.

**5.**

```javascript
let x = 5;
let y = "3";
let result = x + y;
console.log(result);
```

**Answer:** `"53"`

**6.** 15 + 27 = **42**

**7.** ₹350 + ₹45 = **₹395**

**8.** `"25" + 10` = **"2510"**
Because `+` joins them as strings.

**9.**

```javascript
750 + 320 = 1070
2000 - 1070 = 930
```

**Answer:** Total spent = **₹1070**
Remaining = **₹930**

**10.**

```javascript
console.log(5 + "5" + 5);
```

**Answer:** `"555"`

```javascript
console.log(5 + 5 + "5");
```

**Answer:** `"105"`

```javascript
console.log("5" + 5 + 5);
```

**Answer:** `"555"`

---

## 2. Subtraction (-)

**1.** 80 - 53 = **27 seats**

**2.** 500 - 35 = **465 marks**

**3.** 2500 - 875 = **1625 boxes**

**4.**

```javascript
let a = "10";
let b = 3;
let result = a - b;
console.log(result);
```

**Answer:** **7**

**5.**

```javascript
let x = "20";
let y = "5";
let result = x - y;
console.log(result);
```

**Answer:** **15**

**6.** 100 - 37 = **63**

**7.** 500 - 175 = **325 litres**

**8.**

```javascript
"50" - 20 = 30
"50" - "20" = 30
```

**Answer:** Both give **30** because `-` converts strings to numbers.

**9.**

```javascript
240 - 95 - 67 = 78
```

**Answer:** **78 apples left**

**10.**

```javascript
console.log("100" - 50);
```

**Answer:** **50**

```javascript
console.log("abc" - 10);
```

**Answer:** **NaN**

```javascript
console.log(10 - "5" - "2");
```

**Answer:** **3**

```javascript
console.log("10" - "5" - "2");
```

**Answer:** **3**

---

## 3. Multiplication (*)

**1.** 45 × 8 = **₹360**

**2.** 120 × 6 = **720 bottles**

**3.** 7 × 15 = **105 plants**

**4.**

```javascript
let a = "5";
let b = 4;
let result = a * b;
console.log(result);
```

**Answer:** **20**

**5.**

```javascript
let x = "10";
let y = "2";
let result = x * y;
console.log(result);
```

**Answer:** **20**

**6.** 12 × 8 = **96**

**7.** 299 × 4 = **₹1196**

**8.**

```javascript
"7" * 6 = 42
"7" * "6" = 42
```

**Answer:** Both are **42**.

**9.**

```javascript
45 * 8 = 360
```

**Answer:** **360 units**

**10.**

```javascript
console.log("5" * 3 * "2");
```

**Answer:** **30**

```javascript
console.log("abc" * 4);
```

**Answer:** **NaN**

```javascript
console.log(10 * "2.5");
```

**Answer:** **25**

```javascript
console.log("10" * "2.5" * "0");
```

**Answer:** **0**

---

## 4. Division (/)

**1.** 144 ÷ 12 = **12 pencils**

**2.** 360 ÷ 6 = **60 km/hour**

**3.** ₹72,000 ÷ 9 = **₹8,000**

**4.**

```javascript
let a = "20";
let b = 4;
let result = a / b;
console.log(result);
```

**Answer:** **5**

**5.**

```javascript
let x = "100";
let y = "5";
let result = x / y;
console.log(result);
```

**Answer:** **20**

**6.** 144 ÷ 12 = **12**

**7.** 360 ÷ 9 = **40 students**

**8.**

```javascript
"100" / 4 = 25
"100" / "4" = 25
```

**Answer:** Both are **25**.

**9.**

```javascript
2400 / 6 = 400
```

**Answer:** Each friend gets **₹400**

**10.**

```javascript
console.log(10 / 0);
```

**Answer:** **Infinity**

```javascript
console.log(-10 / 0);
```

**Answer:** **-Infinity**

```javascript
console.log(0 / 0);
```

**Answer:** **NaN**

```javascript
console.log("20" / "4" / 2);
```

**Answer:** **2.5**

```javascript
console.log("abc" / 5);
```

**Answer:** **NaN**

---

## 5. Modulus (%)

**1.** 53 % 5 = **3 students**

**2.** 128 % 10 = **8 candies**

**3.** 237 % 6 = **3 toys**

**4.** 185 % 40 = **25 people**

**5.**

```javascript
let a = 10;
let b = 0;
let result = a % b;
console.log(result);
```

**Answer:** **NaN**

**6.** 29 % 5 = **4**

**7.** 23 % 4 = **3 chocolates**

**8.**

```javascript
0 % 7 = 0
15 % 0 = NaN
```

**9.**

```javascript
47 / 6 = 7.83
47 % 6 = 5
```

**Answer:** **7 full sheets and 5 pages left.**

**10.**

```javascript
console.log(17 % 5);
```

**Answer:** **2**

```javascript
console.log(-17 % 5);
```

**Answer:** **-2**

```javascript
console.log(17 % -5);
```

**Answer:** **2**

```javascript
console.log(-17 % -5);
```

**Answer:** **-2**

```javascript
console.log(10 % 0);
```

**Answer:** **NaN**

---

## 6. Exponentiation (**)

**1.** 6 ** 3 = **216 cm³**

**2.** 9 ** 2 = **81 cells**

**3.** 5 ** 4 = **625**

**4.** 1024 ** 2 = **1,048,576 pixels**

**5.**

```javascript
let base = 2;
let power = -1;
let result = base ** power;
console.log(result);
```

**Answer:** **0.5**

**6.** 3 ** 4 = **81**

**7.** 9 ** 2 = **81 square units**

**8.**

```javascript
2 ** 5 = 32
5 ** 2 = 25
```

**Answer:** **No, they are not the same.**

**9.**

```javascript
console.log(2 ** 3 ** 2);
```

**Answer:** **512**

```javascript
console.log((2 ** 3) ** 2);
```

**Answer:** **64**

```javascript
console.log(2 ** -3);
```

**Answer:** **0.125**

```javascript
console.log(-2 ** 2);
```

**Answer:** **Syntax Error**

```javascript
console.log((-2) ** 2);
```

**Answer:** **4**

```javascript
console.log(4 ** 0.5);
```

**Answer:** **2**

**10.**

```javascript
let a = 10;
let b = 0;
let result = a ** b;
console.log(result);
```

**Answer:** **1**
