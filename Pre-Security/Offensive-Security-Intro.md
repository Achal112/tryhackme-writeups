# Offensive Security Intro

## Platform
TryHackMe

---

## Objective
Understand the basics of offensive security by simulating attacks on a vulnerable web application.

---

## What is Offensive Security?
Offensive Security involves thinking like an attacker to find vulnerabilities before real hackers do.

---

## Lab Overview
In this lab, a vulnerable banking application (**FakeBank**) is used to simulate real-world attack scenarios.

---

## Methodology
The approach followed in this lab:
1. Reconnaissance – Understanding the application
2. Enumeration – Discovering hidden resources
3. Exploitation – Using vulnerabilities to perform actions

---

## Task 1: Think Like a Hacker

### Screenshots:
![image](../images/ans1.png)

**Question:**  
Which term describes simulating a hacker's actions?

**Answer:**  
`Offensive Security`

---

## Task 2: Starting the Lab

### Screenshots:
![task1](../images/ans2.png)

- Launched FakeBank application
- Observed account details

**Answer:**  
`8881`

---

## Task 3: Find Hidden Pages

### Screenshots:
![task2](../images/ans3.png)

### Command Used:
```bash
dirb http://fakebank.thm
```
### Discovered URLs:
/images
/bank-transfer

### Explanation:

The ```dirb``` tool performs directory brute-forcing to discover hidden endpoints that are not directly visible on the website.

### Answer:
```bash
http://fakebank.thm/bank-transfer
```

---

## Task 4: Attack the Admin Page

### Screenshots:
![task3](../images/ans4-1.png)

### Steps:

1. Navigate to:
```bash
  http://fakebank.thm/bank-transfer
```
2. Select account: 8881
3. Enter amount: 2000
4. Click Deposit Money

### Screenshots:
![image](../images/ans4-2.png)

### 🎉 Result:
Popup appeared with flag.

### Flag:
```bash
BANK-HACKED
```

---

## Key Learnings
- Offensive security focuses on finding system weaknesses
- Hidden directories can expose sensitive functionality
- Tools like dirb help discover hidden endpoints
- Poor access control can lead to serious vulnerabilities

---

### Vulnerability Identified
- Unprotected admin endpoint (/bank-transfer)
- Lack of authentication and authorization controls

## Tools Used
- dirb
- Linux Terminal

---

## Conclusion

This lab demonstrated how attackers enumerate hidden directories and exploit exposed functionality to manipulate a web application. It highlights the importance of securing endpoints and implementing proper access controls.
