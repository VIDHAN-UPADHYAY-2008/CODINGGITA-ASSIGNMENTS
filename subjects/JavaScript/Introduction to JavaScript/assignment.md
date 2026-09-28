# Assignment: Introduction to JavaScript

## Section A: Short Answer Questions

**Q1. What is JavaScript?**
JavaScript is a high-level programming language used to make web pages interactive and dynamic.

**Q2. Who created JavaScript and in which year?**
JavaScript was created by **Brendan Eich in 1995**.

**Q3. What was the original name of JavaScript?**
Its original name was **Mocha**. It was later called LiveScript and then JavaScript.

**Q4. Is JavaScript the same as Java?**
No. JavaScript and Java are different languages. JavaScript is mainly used for web development, while Java is a general-purpose programming language.

**Q5. What does high-level mean?**
It means the language is easy for humans to understand and hides complex computer details.

**Q6. Is JavaScript compiled or interpreted?**
JavaScript is commonly called an interpreted language, but modern engines use **Just-In-Time (JIT) compilation** to execute it efficiently.

**Q7. JavaScript engines:**

* Chrome → **V8**
* Firefox → **SpiderMonkey**
* Safari → **JavaScriptCore**

**Q8. What is Dynamic Typing?**
Dynamic typing means a variable can store different types of values at different times.

**Q9. Static vs Dynamic website:**
A static website shows mostly fixed content, while a dynamic website can change content based on users or data.

**Q10. Three pillars of Front-end Development:**

* **HTML** → Structure of webpage.
* **CSS** → Design and appearance.
* **JavaScript** → Behaviour and interaction.

**Q11. Frontend vs Backend:**
Frontend is what the user sees and uses. Backend works behind the scenes with servers, databases, and application logic.

**Q12. What is Node.js?**
Node.js is a runtime that allows JavaScript to run outside a web browser, especially on servers.

**Q13. What is ECMAScript?**
ECMAScript is the standard specification that defines JavaScript features and rules. JavaScript is an implementation of ECMAScript.

---

# Section B: True or False

**1.** False — JavaScript is dynamically typed.
**2.** False — JavaScript can also run outside browsers using environments like Node.js.
**3.** False — JavaScript is mainly responsible for webpage behaviour.
**4.** True.
**5.** False — JavaScript is case-sensitive.
**6.** False — `name` and `Name` are different variables.
**7.** False — ECMAScript is a standard/specification, not a programming language.
**8.** False — React, Angular, and Vue.js are mainly used for frontend development.

---

# Section C: Fill in the Blanks

**1.** JavaScript was created by **Brendan Eich** in **1995**.

**2.** **HTML, CSS, and JavaScript**

**3.** Chrome uses **V8**, Firefox uses **SpiderMonkey**.

**4.** Customer = **Frontend**, Waiter = **API**, Chef = **Backend**.

**5.** **`.js`**

---

# Section D: Conceptual Questions

**Q14. Static vs Dynamic Website**

A **static website** displays fixed content. Example: a simple portfolio page.
A **dynamic website** can change content based on users or data. Example: YouTube.

**Q15. Two features of JavaScript**

1. **Event handling** — responds to clicks, typing, etc.
2. **DOM manipulation** — can change webpage content and styles.

**Q16. Four areas where JavaScript is used**

1. **Backend** → Node.js
2. **Mobile apps** → React Native
3. **Desktop apps** → Electron
4. **Game development** → Phaser

**Q17. Internal vs External JavaScript**

**Internal:** JavaScript is written inside `<script>` in the HTML file.
**External:** JavaScript is written in a separate `.js` file.

Advantages of external JavaScript:

1. Code can be reused on multiple pages.
2. HTML remains cleaner and easier to maintain.

**Q18. Frontend and Backend — Restaurant Analogy**

Frontend is like the **dining area and menu** that customers see and use.
Backend is like the **kitchen**, where the actual work happens.
The waiter/API connects the customer with the kitchen.

**Q19. Why should a beginner learn JavaScript?**

1. It is widely used in web development.
2. It makes websites interactive.
3. It can be used for frontend and backend.
4. It has many libraries and frameworks.
5. It provides many career opportunities.

---

# Section E: Code-Based Questions

**Q20. Output**

```text
number
string
boolean
```

**Why?**
The `typeof` operator tells the type of the current value. The variable changes from a number to a string and then to a boolean.

---

**Q21. Alert on button click**

```html
<!DOCTYPE html>
<html>
<body>

<button onclick="alert('Welcome to JavaScript!')">
  Click Me
</button>

</body>
</html>
```

---

**Q22. Event-driven programming**

```html
<!DOCTYPE html>
<html>
<body>

<p id="demo">Click the button</p>
<button id="myBtn">Click Me</button>

<script>
document.getElementById("myBtn").onclick = function() {
  document.getElementById("demo").textContent = "Button was clicked!";
};
</script>

</body>
</html>
```

---

# Section F: Practical / Application Based

**Q23. Complete Web Page**

```html
<!DOCTYPE html>
<html>
<head>
  <title>My First JavaScript Page</title>
</head>

<body>

<h1>My First JavaScript Page</h1>

<button id="btn">Click Me</button>

<script>
console.log("JavaScript is running successfully!");

document.getElementById("btn").onclick = function() {
  alert("Hello, B.Tech Student!");
  document.body.style.backgroundColor = "lightblue";
};
</script>

</body>
</html>
```


# Section G: Higher Order Thinking

**Q24. Why did JavaScript become popular?**

JavaScript became popular because it is easy to use and works across many platforms. It can be used for websites, servers, mobile apps, and desktop apps. **Node.js** allowed JavaScript to run outside browsers. **ECMAScript updates** added new features and improved JavaScript over time. Its large ecosystem also helped it grow.
