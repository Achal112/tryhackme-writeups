# 🌐 DNS Fundamentals – TryHackMe Write-up

## Room Information

* **Platform:** TryHackMe
* **Room Name:** DNS Fundamentals
* **Difficulty:** Beginner
* **Status:** ✅ Completed

---

## Objective

Learn how DNS works, including domain structure, record types, and how DNS queries are resolved.

---

# Task 1: What is DNS?

![task1](images/ans1.png)

---

DNS provides a way to translate human-readable domain names into IP addresses.

👉 Example:

* `tryhackme.com` → `104.26.10.229`

### ✅ Answer:

`Domain Name System`

---

# Task 2: Domain Hierarchy

![task2](images/ans2-1.png)
![task2](images/ans2-2.png)

---

### 🔹 Structure:

* **TLD (Top-Level Domain):** `.com`, `.org`, `.in`
* **Second-Level Domain:** `tryhackme`
* **Subdomain:** `admin.tryhackme.com`

---

![task2](images/ans2-3.png)

---

### ✅ Answers:

* Maximum subdomain length → `63`
* Invalid character → `_`
* Maximum domain length → `253`
* `.co.uk` type → `ccTLD`

---

# Task 3: DNS Record Types

![task3](images/ans3-1.png)

---

### 🔹 Common Records:

* **A Record:** Maps to IPv4
* **AAAA Record:** Maps to IPv6
* **CNAME Record:** Maps to another domain
* **MX Record:** Mail servers
* **TXT Record:** Text-based data

---

![task3](images/ans3-2.png)

---

### ✅ Answers:

* Record for email → `MX`
* Record for IPv6 → `AAAA`

---

# Task 4: DNS Request Flow

![task4](images/ans4-1.png)

---

### Steps:

1. Local cache check
2. Recursive DNS server
3. Root server
4. TLD server
5. Authoritative server
6. Response returned + cached

---

![task4](images/ans4-2.png)

---

### ✅ Answers:

* Cache duration → `TTL`
* ISP provides → `Recursive DNS Server`
* Stores records → `Authoritative DNS Server`

---

# Task 5: Practical DNS Queries

![task5](images/ans5-1.png)

---

### 🔹 CNAME Record:

- Set the DNS query to CNAME
- Set the subdomain to shop

```bash
shops.myshopify.com
```

---

![task5](images/ans5-2.png)

---

### 🔹 TXT Record:

- Set the DNS query to TXT
- Set the subdomain blank

```bash
THM{7012BBA60997F35A9516C2E16D2944FF}
```

---

![task5](images/ans5-3.png)

---

### 🔹 MX Priority:

- Set the DNS query to MX
- Set the subdomain blank

```bash
30
```

---

![task5](images/ans5-4.png)

---

### 🔹 A Record IP:

- Set the DNS query to A
- Set the subdomain to www

```bash
10.10.10.10
```

---

# Final Outcome

Successfully understood:

* DNS structure
* Record types
* DNS resolution process
* Practical DNS queries

---

# Skills Gained

* DNS enumeration
* Understanding DNS hierarchy
* Identifying DNS records
* Basic reconnaissance skills

---

# Real-World Relevance

DNS is critical in:

* Penetration Testing
* Bug Bounty Hunting
* Network Security
* SOC Operations

---

# Challenges Faced

* Understanding DNS resolution flow
* Remembering record types

---


# Author

**Achal Deshmukh**

* 🎓 MCA Student
* 🔐 Cybersecurity Learner

---

# ⭐ Notes

DNS is a common attack surface in cybersecurity, often targeted for spoofing, phishing, and misconfiguration exploitation.
