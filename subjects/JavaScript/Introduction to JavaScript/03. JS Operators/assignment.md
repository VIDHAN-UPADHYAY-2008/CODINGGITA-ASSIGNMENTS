Assignment: JavaScript Operators
A] Arithmetic Operators
1. Addition (+)

₹27,500

43 pages

303 items

"105"

"53"

42

₹395

"2510" — String concatenation.

Spent = ₹1,070; Balance = ₹930

"555", "105", "555"

2. Subtraction (-)

27 seats

465 marks

1,625 boxes

7

15

63

325 litres

Both 30

240 - 95 - 67 = 78

50, NaN, 3, 3

3. Multiplication (*)

₹360

720 bottles

105 plants

20

20

96

₹1,196

Both 42

45 * 8 = 360

30, NaN, 25, 0

4. Division (/)

12 pencils

60 km/hour

₹8,000

5

20

12

40 students

Both 25

₹400

Infinity, -Infinity, NaN, 2.5, NaN

5. Modulus (%)

3 students

8 candies

3 toys

25 people

NaN

4

3 chocolates

0, NaN

7 full sheets, 5 pages left

2, -2, 2, -2, NaN

6. Exponentiation (**)

216 cm³

81 cells

625

1,048,576 pixels

0.5

81

81 square units

32, 25; No

512, 64, 0.125, SyntaxError, 4, 2

1

B] Assignment Operators
1. Simple Assignment (=)

let name = "Priya", marks = 92;

let score = 0;

let a = 50, b = 50, c = 50;

100

15 30

2. Add and Assign (+=)

105

1620

15

"Good Morning"

"205" — String concatenation.

3. Subtract and Assign (-=)

65

255

3

25

NaN

4. Multiply and Assign (*=)

590

24

220.00000000000003

21

NaN

5. Divide and Assign (/=)

30

60

50

25

Infinity

6. Modulus and Assign (%=)

5

11

4

2

NaN

7. Exponentiation and Assign (**=)

125

16

32

2

0.5

C] Comparison Operators
1. Loose Equality (==)

true

true

true, true

true, true

false — NaN is not equal to itself.

2. Loose Inequality (!=)

false

false

false, false

false, false

true

3. Strict Equality (===)

false — Different types.

false, false

false, false

false, false

Prevents automatic type conversion.

4. Strict Inequality (!==)

true

true, true

true, true

true, true

input !== "0"

Part C] Relational Operators


5. Greater Than (>)

• Q: Marks 78, passing 40. Check if student scored more than passing marks.
	• A: 78 > 40 \(\rightarrow \) true
	
• Q: Temp today 35°C, yesterday 28°C. Check if today is hotter.
	• A: 35 > 28 \(\rightarrow \) true
• Q: Predict output: console.log(15 > 10); console.log(10 > 15); console.log(10 > 10);
	• A: true, false, false
	
• Q: Predict output: console.log("20" > 15); console.log("5" > "10"); console.log("abc" > 10);
	• A: true (string "20" becomes number 20), true (alphabetical comparison: "5" comes after "1"), false ("abc" becomes NaN, any comparison with NaN is false)
	
• Q: Result of null > 0 and undefined > 0? Explain.
	• A: Both are false. null becomes 0 (\(0 > 0\) is false). undefined becomes NaN, which always returns false.
	
• Q: Stock 120, customer wants 85. Condition using > to check if stock is sufficient.
	• A: 120 >= 85 (or 120 > 84)
	
• Q: Predict and explain: console.log(true > false); console.log("10" > "2"); console.log(NaN > 5);
	• A:
		• true (true becomes 1, false becomes 0, so \(1 > 0\))
		• false (string comparison looks at first characters: "1" is smaller than "2")
		• false (NaN comparisons are always false)
		

6. Less Than (<)

• Q: Box max 50 kg, current 42 kg. Check if more items can be added.
	• A: 42 < 50 \(\rightarrow \) true
	
• Q: Age 16, min required 18. Check if person is underage.
	• A: 16 < 18 \(\rightarrow \) true
	
• Q: Predict output: console.log(8 < 12); console.log(20 < 10); console.log(7 < 7);
	• A: true, false, false
	
• Q: Predict output: console.log("8" < 10); console.log("20" < "3"); console.log("hello" < 5);
	• A: true ("8" becomes number 8), true (string comparison: "2" comes before "3"), false ("hello" becomes NaN)
	
• Q: Result of null < 0 and undefined < 0? Explain.
	• A: Both are false. null becomes 0 (\(0 < 0\) is false). undefined becomes NaN (always false).
	
• Q: Tank capacity 500L, current 375L. Condition using < to check if not full.
	• A: 375 < 500
	
• Q: Predict and explain: console.log(false < true); console.log("5" < "15"); console.log(NaN < 10);

	• A:
	
		• true (\(0 < 1\))
		• false (string comparison: "5" comes after "1")
		• false (NaN makes it false)

7. Greater Than or Equal To (>=)

• Q: Distinction 75, student scored 75. Check if they get distinction.
	• A: 75 >= 75 \(\rightarrow \) true
	
• Q: Ticket ₹300, person has ₹300. Check if they can buy.
	• A: 300 >= 300 \(\rightarrow \) true
	
• Q: Predict output: console.log(25 >= 25); console.log(30 >= 25); console.log(20 >= 25);
	• A: true, true, false
	
• Q: Predict output: console.log("25" >= 25); console.log("10" >= "2"); console.log(null >= 0);
	• A: true (converts to number), false (string "1" is smaller than "2"), true (null becomes 0, and \(0 \geq 0\) is true)
	
• Q: Result of undefined >= 0? Explain.
	• A: false. undefined becomes NaN, and NaN is never greater than or equal to anything.
	
• Q: Lift max 8 people, current 8 people. Condition using >= to check if full/overloaded.
	• A: 8 >= 8
	
• Q: Predict and explain: console.log(true >= 1); console.log("" >= 0); console.log(NaN >= NaN);

	• A:
		• true (true becomes 1, so \(1 \geq 1\))
		
		• true (empty string "" becomes 0, so \(0 \geq 0\))
		
		• false (NaN is never equal to or greater than anything, even itself)
		

8. Less Than or Equal To (<=)

• Q: Max speed limit 60, vehicle going 60. Check if within limit.

	• A: 60 <= 60 \(\rightarrow \) true
• Q: Needs 40 to pass, scored 39. Check if failed.

	• A: 39 < 40 (or 39 <= 39) \(\rightarrow \) true
• Q: Predict output: console.log(15 <= 20); console.log(20 <= 15); console.log(15 <= 15);

	• A: true, false, true
• Q: Predict output: console.log("15" <= 20); console.log("30" <= "5"); console.log(null <= 0);

	• A: true (converts to number), true (string "3" comes before "5"), true (null becomes 0, so \(0 \leq 0\))
• Q: Result of undefined <= 0? Explain.

	• A: false. undefined becomes NaN, which fails all relative comparisons.
• Q: Bag max 10 books, current 10 books. Condition using <= to check if more books can be added.

	• A: 10 < 10 (returns false, meaning no room left) or to check if it's already full: 10 >= 10.
• Q: Predict and explain: console.log(false <= 0); console.log("" <= 0); console.log(NaN <= 5);

	• A:
		• true (false becomes 0, so \(0 \leq 0\))
		• true ("" becomes 0, so \(0 \leq 0\))
		• false (contains NaN)

Mixed Practice (>, <, >=, <=)


• Q: Write expressions to check:

	• Age 18 \(\ge \) voting age 18: 18 >= 18
	• Temp 32 < 35: 32 < 35
	• Score 90 > 85: 90 > 85
• Q: Predict outputs:

	• console.log(10 > 5 && 5 < 10); \(\rightarrow \) true (true && true)
	
	• console.log("10" >= 10); \(\rightarrow \) true (number 10 equals 10)
	
	• console.log(null <= undefined); \(\rightarrow \) false (undefined turns to NaN)
	
	• console.log("5" < "10" && 5 > 2); \(\rightarrow \) false (string "5" < "10" is false because "5" > "1")
	
• Q: Product costs ₹499, customer has ₹500. Write conditions using >= and < to decide if they can buy and if change is left.

	• Can buy: 500 >= 499
	
	• Change left: 499 < 500
	
• Q: Explain why "10" > "2" is false but 10 > 2 is true.

	• A: "10" > "2" compares strings alphabetically character-by-character; the character "1" comes before "2", making it false. 10 > 2 compares actual numerical values, so it is true.
	
