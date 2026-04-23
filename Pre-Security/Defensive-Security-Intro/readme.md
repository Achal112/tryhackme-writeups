# 🛡️ Defensive Security Intro

## Platform
TryHackMe

---

## Objective
Understand the fundamentals of defensive security, including detecting, analyzing, and responding to cyber attacks.

---

## What is Defensive Security?
Defensive Security focuses on protecting systems by monitoring, detecting, and responding to cyber threats. Unlike offensive security, it does not involve attacking systems but securing them against attacks.

---

## Lab Overview
In this lab, we act as a defender protecting a vulnerable banking application (**FakeBank**) from an ongoing cyber attack. The goal is to detect suspicious activity, identify the attack, and stop it.

---

## Methodology
The approach followed in this lab:
1. Monitoring system activity  
2. Detecting suspicious behavior  
3. Investigating the attack  
4. Responding to stop the attack  

---

## Task 1: Think Like a Defender

### Screenshot:
![task1](https://raw.githubusercontent.com/Achal112/tryhackme-writeups/refs/heads/main/Pre-Security/images/res1.png)

---

**Question:**  
What is the main goal of defensive security?

**Answer:**  
`Detect and respond to attacks`

---

## Task 2: Detect Suspicious Activity

### Objective:
- Identify the suspicious source IP from the monitoring dashboard.

---

### Investigation Steps:
1. Opened the monitoring dashboard  
2. Reviewed recent alerts and logs  
3. Analyzed source IP activity  

---

### Screenshot:
![task2](https://raw.githubusercontent.com/Achal112/tryhackme-writeups/refs/heads/main/Pre-Security/images/res2.png)


---


### Observations:
- One IP address was making repeated requests  
- High number of failed login attempts were observed  
- Activity pattern indicated possible brute-force attack  

---

### Suspicious IP:
```bash
32.122.195.63
```

### Explanation:
The identified IP showed abnormal behavior compared to normal users. The high frequency of requests and repeated failures indicate malicious activity.

---

## Task 3: Identify the Attack

### Objective:
Determine the type of attack by analyzing the attacker's activity in the monitoring dashboard.

---

### Investigation Steps:
1. Opened the monitoring dashboard  
2. Navigated to the **"URL Discovery Attempts"** section  
3. Reviewed the latest entries  

---

### Screenshot:
![task3](https://raw.githubusercontent.com/Achal112/tryhackme-writeups/refs/heads/main/Pre-Security/images/res3-1.png)


---

### Observation
- The attacker was attempting to access hidden or restricted URLs  
- Multiple URL requests were made in a short period  
- The latest attempt targeted an admin endpoint  

---

### Latest URL Attempted
```bash
https://fakebank.com/admin
```
---

![task3](https://raw.githubusercontent.com/Achal112/tryhackme-writeups/refs/heads/main/Pre-Security/images/res3-2.png)

---

### Analysis
The attacker is performing a **directory enumeration (or URL brute-forcing) attack**, trying to discover hidden endpoints such as admin panels.

---

### Attack Type
- Directory Brute Force  
- Enumeration Attack  

---

### Explanation
Attackers often use automated tools to scan for hidden directories and sensitive endpoints. Access to an admin panel could allow unauthorized control over the system.

---

## Key Learning
- Monitoring URL requests helps detect reconnaissance activity  
- Repeated access attempts to hidden paths indicate malicious intent  
- Early detection prevents further exploitation 

---

## Task 4: Stop the Attack

### Objective
Stop the ongoing attack by blocking the attacker’s IP address.

---

![task4](https://raw.githubusercontent.com/Achal112/tryhackme-writeups/refs/heads/main/Pre-Security/images/res4-1.png)

---

### Action Taken
1. Reviewed security actions in the dashboard  
2. Identified attacker’s IP address:  
```bash
32.122.195.63
```
3. Added a firewall rule to block the IP  
4. Selected **BLOCK** and applied the rule  

---

![task4](https://raw.githubusercontent.com/Achal112/tryhackme-writeups/refs/heads/main/Pre-Security/images/res4-2.png)

---

### Result
The attacker’s IP was successfully blocked, preventing further malicious activity.

---

![task4](https://raw.githubusercontent.com/Achal112/tryhackme-writeups/refs/heads/main/Pre-Security/images/res4-3.png)

---

### Flag
THM{FAKEBANK-SECURED} ```

---

### Explanation
Blocking the attacker’s IP is a form of incident response (containment). This prevents the attacker from continuing their actions and protects the system from further damage.

---

### Security Concept
- Firewall Rule Implementation
- Incident Response (Containment Phase)

---

### Key Learning
- Quick response is critical during an attack
+ Firewalls are essential for blocking malicious traffic
- Identifying and stopping attackers reduces system risk

---

## Key Concepts

- **Monitoring:** Continuously observing system activity  
- **Detection:** Identifying suspicious behavior  
- **Response:** Taking action to stop attacks  

---

## Key Learnings
- Defensive security focuses on protection, not attack  
- Early detection is critical to prevent damage  
- Logs and monitoring tools are essential for identifying threats  
- Quick response reduces the impact of attacks  

---

## Tools & Concepts Used
- Log Analysis  
- Monitoring Systems  
- Incident Response  

---

## Conclusion
This lab demonstrated how defenders monitor systems, detect suspicious activity, analyze threats, and respond effectively to stop cyber attacks.

---

## Disclaimer
This lab was performed in a legal environment provided by TryHackMe.  
This writeup is for educational purposes only.

---

## Real-World Relevance
In real organizations, defensive security is implemented using Security Operations Centers (SOC), where analysts monitor logs, detect threats, and respond to incidents in real time.
