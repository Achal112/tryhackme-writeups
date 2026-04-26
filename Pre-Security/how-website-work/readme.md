# How Websites Work – TryHackMe Write-up

## Room Information

* **Platform:** TryHackMe
* **Room Name:** How Websites Work
* **Difficulty:** Beginner
* **Status:** ✅ Completed

---

## Objective

Understand how websites function, including:

* Frontend vs Backend
* HTML structure
* JavaScript basics
* Common web vulnerabilities

---

# Task 1: How Websites Work

When a user visits a website:

* Browser sends a request to a web server
* Server responds with data
* Browser renders the page

---

### 🔹 Components:

* **Front End (Client-side):** Display in browser
* **Back End (Server-side):** Processes requests

---

### ✅ Answer:

* Component rendered in browser → `Front End`

---

# Task 2: HTML

### 🔹 What is HTML?

HTML (HyperText Markup Language) is used to structure web pages.

---

### 🔹 Basic Structure:

```html id="h8z2zt"
<!DOCTYPE html>
<html>
<head>
    <title>Page Title</title>
</head>
<body>
    <h1>Heading</h1>
    <p>Paragraph</p>
</body>
</html>
```

---

### 🔹 Key Concepts:

* Tags (`<p>`, `<h1>`, `<img>`)
* Attributes (`src`, `class`, `id`)
* `id` is unique, `class` can repeat

---

### Practical Tasks:

* Fixed broken image
* Added new `<img>` tag

---

### ✅ Answers:

* Hidden text → `HTMLHERO`
* Dog image text → `DOGHTML`

---

# Task 3: JavaScript

### 🔹 What is JavaScript?

JavaScript adds interactivity to web pages.

---

### 🔹 Example:

```javascript id="n3b9q2"
document.getElementById("demo").innerHTML = "Hack the Planet";
```

---

### 🔹 Events Example:

```html id="m7cxqk"
<button onclick='document.getElementById("demo").innerHTML = "Button Clicked";'>
Click Me!
</button>
```

---

### Practical Task:

* Modified content using JS
* Added interactive button

---

### ✅ Answer:

* Flag → `JSISFUN`

---

# Task 4: Sensitive Data Exposure

### 🔹 Concept:

Sensitive data exposed in:

* HTML source code
* JavaScript files
* Comments

---

### 🔹 Example:

* Hardcoded credentials
* Hidden links

---

### ✅ Answer:

* Password found → `testpasswd`

---

# Task 5: HTML Injection

### 🔹 Concept:

Occurs when user input is not sanitized.

👉 Attacker can inject:

* HTML
* JavaScript

---

### 🔹 Risk:

* Modify page content
* Phishing attacks
* Script execution

---

### Practical Task:

Injected malicious link into page.

---

### ✅ Answer:

* Flag → `HTML_INJ3CTI0N`

---

# Final Outcome

Successfully learned:

* How websites work (frontend & backend)
* HTML and JavaScript basics
* Common vulnerabilities (data exposure, injection)

---

# Skills Gained

* Basic web development understanding
* HTML & JS fundamentals
* Identifying frontend vulnerabilities
* Security mindset for web apps

---

# Real-World Relevance

This knowledge is essential for:

* Web Penetration Testing
* Bug Bounty Hunting
* Secure Web Development
* SOC Analysis

---

# Challenges Faced

* Understanding HTML structure initially
* Learning how JS manipulates DOM
* Recognizing injection vulnerabilities

---

# 🚀 Author

**Achal Deshmukh**

* 🎓 MCA Student
* 🔐 Cybersecurity Learner

---

# ⭐ Notes

Understanding how websites work is the foundation for both **web development and web security**, especially when identifying vulnerabilities like injection and sensitive data exposure.
