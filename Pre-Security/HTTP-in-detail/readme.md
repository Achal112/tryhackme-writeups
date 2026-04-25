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

### 🔹 HTTP

HTTP (HyperText Transfer Protocol) is used for communication between web clients and servers.

### 🔹 HTTPS

HTTPS is the secure version of HTTP using encryption.

---

### ✅ Answers:

* HTTP stands for → `HyperText Transfer Protocol`
* HTTPS “S” stands for → `Secure`
* Flag → `THM{INVALID_HTTP_CERT}`

---

# Task 2: URLs & Requests

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

### ✅ Answers:

* Protocol used → `HTTP/1.1`
* Header for data size → `Content-Length`

---

# Task 3: HTTP Methods

### 🔹 Common Methods:

* **GET** → Retrieve data
* **POST** → Create data
* **PUT** → Update data
* **DELETE** → Remove data

---

### ✅ Answers:

* Create user → `POST`
* Update email → `PUT`
* Delete data → `DELETE`
* View article → `GET`

---

# Task 4: HTTP Status Codes

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

### ✅ Answers:

* New resource → `201`
* Page not found → `404`
* Server issue → `503`
* Unauthorized → `401`

---

# Task 5: HTTP Headers

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

### ✅ Answers:

* Browser info → `User-Agent`
* Data type → `Content-Type`
* Website → `Host`

---

# Task 6: Cookies

### 🔹 Concept:

Cookies store small data on the client to maintain session state.

* Used for authentication
* Stored via `Set-Cookie` header
* Sent back in future requests

---

### ✅ Answer:

* Cookie header → `Set-Cookie`

---

# Task 7: Practical HTTP Requests

### 🔹 GET /room

```bash
THM{YOU'RE_IN_THE_ROOM}
```

---

### 🔹 GET /blog?id=1

```bash
THM{YOU_FOUND_THE_BLOG}
```

---

### 🔹 DELETE /user/1

```bash
THM{USER_IS_DELETED}
```

---

### 🔹 PUT /user/2 (username=admin)

```bash
THM{USER_HAS_UPDATED}
```

---

### 🔹 POST /login (thm / letmein)

```bash
THM{HTTP_REQUEST_MASTER}
```

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
