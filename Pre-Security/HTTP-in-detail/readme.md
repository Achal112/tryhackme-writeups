# HTTP Fundamentals – TryHackMe Write-up

## Room Information

* **Platform:** TryHackMe
* **Room Name:** HTTP Fundamentals
* **Difficulty:** Beginner
* **Status:** ✅ Completed

---

## Objective

Understand how HTTP/HTTPS works, including:

* Web communication basics
* HTTP requests & responses
* Methods & status codes
* Headers & cookies
* Practical HTTP interaction

---

# Task 1: What is HTTP / HTTPS?

---

![task1](images/res1-1.png)
![task1](images/res1-2.png)

---

### 🔹 HTTP

HTTP (HyperText Transfer Protocol) is used for communication between web clients and servers.

### 🔹 HTTPS

HTTPS is the secure version of HTTP using encryption.

---

![task1](images/res1-3.png)

---

### ✅ Answers:

* HTTP stands for → `HyperText Transfer Protocol`
* HTTPS “S” stands for → `Secure`
* Flag → `THM{INVALID_HTTP_CERT}`

---

# Task 2: URLs & Requests

---

![task2](images/res2-1.png)
![task2](images/res2-2.png)
![task2](images/res2-3.png)
![task2](images/res2-4.png)

---

### 🔹 URL Components:

* Scheme → HTTP / HTTPS
* Host → Domain name
* Port → 80 (HTTP), 443 (HTTPS)
* Path → Resource location
* Query → Parameters
* Fragment → Page section

---

### 🔹 Example Request:

```http
GET / HTTP/1.1
Host: tryhackme.com
User-Agent: Mozilla/5.0
Referer: https://tryhackme.com/
```

---

### 🔹 Example Response:

* Status: `200 OK`
* Header: `Content-Type`, `Content-Length`

---

![task2](images/res2-5.png)

---

### ✅ Answers:

* Protocol used → `HTTP/1.1`
* Header for data size → `Content-Length`

---

# Task 3: HTTP Methods

---

![task3](images/res3-1.png)

---

### 🔹 Common Methods:

* **GET** → Retrieve data
* **POST** → Create data
* **PUT** → Update data
* **DELETE** → Remove data

---

![task3](images/res3-2.png)

---

### ✅ Answers:

* Create user → `POST`
* Update email → `PUT`
* Delete data → `DELETE`
* View article → `GET`

---

# Task 4: HTTP Status Codes

---

![task4](images/res4-1.png)
![task4](images/res4-2.png)

---

### 🔹 Categories:

* `100–199` → Informational
* `200–299` → Success
* `300–399` → Redirection
* `400–499` → Client Error
* `500–599` → Server Error

---

### 🔹 Common Codes:

* 200 → OK
* 201 → Created
* 404 → Not Found
* 401 → Unauthorized
* 503 → Service Unavailable

---

![task4](images/res4-3.png)

---

### ✅ Answers:

* New resource → `201`
* Page not found → `404`
* Server issue → `503`
* Unauthorized → `401`

---

# Task 5: HTTP Headers

---

![task5](images/res5-1.png)

---

### 🔹 Request Headers:

* `Host` → Website requested
* `User-Agent` → Browser info
* `Content-Length` → Data size

---

### 🔹 Response Headers:

* `Content-Type` → Data format
* `Set-Cookie` → Store cookies
* `Cache-Control` → Cache timing

---

![task5](images/res5-2.png)

---

### ✅ Answers:

* Browser info → `User-Agent`
* Data type → `Content-Type`
* Website → `Host`

---

# Task 6: Cookies

---

![task6](images/res6-1.png)

---

### 🔹 Concept:

Cookies store small data on the client to maintain session state.

* Used for authentication
* Stored via `Set-Cookie` header
* Sent back in future requests

---

![task6](images/res6-2.png)

---

### ✅ Answer:

* Cookie header → `Set-Cookie`

---

# Task 7: Practical HTTP Requests

---

![task7](images/res7-1.png)

---

### 🔹 GET /room

```bash
THM{YOU'RE_IN_THE_ROOM}
```

---

![task7](images/res7-2.png)

---

### 🔹 GET /blog?id=1

```bash
THM{YOU_FOUND_THE_BLOG}
```

---

![task7](images/res7-3.png)

---

### 🔹 DELETE /user/1

```bash
THM{USER_IS_DELETED}
```

---

![task7](images/res7-4.png)

---

### 🔹 PUT /user/2 (username=admin)

```bash
THM{USER_HAS_UPDATED}
```

---

![task7](images/res7-5.png)

---

### 🔹 POST /login (thm / letmein)

```bash
THM{HTTP_REQUEST_MASTER}
```

---

![task7](images/res7-6.png)

---

# Final Outcome

Successfully learned:

* HTTP/HTTPS communication
* Request & response structure
* Methods and status codes
* Headers and cookies
* Practical API interaction

---

# Skills Gained

* Web request analysis
* Understanding HTTP protocol
* API interaction basics
* Security awareness (certificates, cookies)

---

# Real-World Relevance

This knowledge is essential for:

* Web Penetration Testing
* Bug Bounty Hunting
* API Security Testing
* SOC Analysis

---

# Challenges Faced

* Understanding headers vs body
* Differentiating HTTP methods
* Learning status code meanings

---


# Author

**Achal Deshmukh**

* 🎓 MCA Student
* 🔐 Cybersecurity Learner

---

# ⭐ Notes

HTTP is the backbone of web communication and a major attack surface in cybersecurity, including vulnerabilities like XSS, SQL Injection, and session hijacking.
