# Putting It All Together – TryHackMe Write-up

## Room Information

* **Platform:** TryHackMe
* **Room Name:** Putting It All Together
* **Difficulty:** Beginner
* **Status:** ✅ Completed

---

## Objective

Understand how all web concepts connect together:

* DNS
* HTTP
* Web servers
* Backend & frontend
* Additional components (CDN, WAF, Load Balancer)

---

# Task 1: Putting It All Together

### 🔹 How a Website Works (Simple Flow)

1. You enter a website (e.g., google.com)
2. DNS finds the IP address
3. Browser sends HTTP request
4. Server responds with data
5. Browser displays the website

---

### ✅ Answer:

* No answer required

---

# Task 2: Other Components

### 🔹 Load Balancer

* Distributes traffic across multiple servers
* Prevents overload
* Performs **health checks** to see if servers are working

---

### 🔹 CDN (Content Delivery Network)

* Stores static files (images, CSS, JS)
* Delivers from nearest server → faster loading

---

### 🔹 Database

* Stores user data
* Examples: MySQL, MongoDB

---

### 🔹 WAF (Web Application Firewall)

* Protects website from attacks
* Blocks malicious requests
* Uses rate limiting

---

### ✅ Answers:

* Static file hosting → `CDN`
* Check server alive → `health check`
* Protect from hacking → `WAF`

---

# Task 3: How Web Servers Work

### 🔹 What is a Web Server?

* Software that handles requests and sends responses
* Examples: Apache, Nginx

---

### 🔹 Virtual Hosts

* Allows one server to host multiple websites

---

### 🔹 Static vs Dynamic Content

| Type    | Description                           |
| ------- | ------------------------------------- |
| Static  | Same content every time (images, CSS) |
| Dynamic | Changes based on user input           |

---

### 🔹 Backend vs Frontend

* **Frontend:** What user sees
* **Backend:** Logic running on server

👉 Backend code is NOT visible to user

---

### 🔹 Backend Languages

* Python, PHP, Node.js, etc.

---

### ✅ Answers:

* Multiple sites → `Virtual Hosts`
* Changing content → `Dynamic`
* Backend visible? → `Nay`

---

# Task 4: Final Quiz

### 🔹 Concept:

Arrange steps of how a web request works.

---

### ✅ Flag:

```bash id="c6x7pf"
THM{YOU_GOT_THE_ORDER}
```

---

# Final Outcome

Successfully understood:

* Complete web request lifecycle
* Supporting components (CDN, WAF, Load Balancer)
* Web server working
* Backend vs Frontend

---

# Skills Gained

* Web architecture understanding
* Networking + HTTP integration
* Basic security awareness
* System design basics

---

# Real-World Relevance

This knowledge is useful for:

* Web Development
* Backend Development
* Cybersecurity (Web Pentesting)
* System Design

---

# Challenges Faced

* Connecting all concepts together
* Understanding request flow

---

# 🚀 Author

**Achal Deshmukh**

* 🎓 MCA Student
* 🔐 Cybersecurity Learner

---

# ⭐ Notes

This room connects all previous concepts and gives a complete understanding of how the web works from request to response.
