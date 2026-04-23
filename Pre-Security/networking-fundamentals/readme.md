# Networking Fundamentals – TryHackMe Write-up

## Room Information

* **Platform:** TryHackMe
* **Room Type:** Pre Security / Networking Basics
* **Difficulty:** Beginner
* **Status:** ✅ Completed

---

## Objective

Understand the fundamentals of computer networking, including:

* What networks are
* How the Internet works
* Device identification (IP & MAC)
* Basic network tools like ping

---

## Task 1: 

[!task1](images/task1-1.png)

### 🔹 What is a Network?

A network is a collection of connected devices that can communicate with each other.

**Answer:** `Network`

---

## Task 2:

[!task2](images/task1-2.png)

### 🔹 What is the Internet?

The Internet is a **global network of networks**, connecting private and public networks worldwide.

**Inventor of WWW:** `Tim Berners-Lee`

---

## Device Identification

Devices on a network are identified using:

### 🔸 IP Address (Logical Identity)

* Stands for: `Internet Protocol`
* Used to identify a device on a network
* Can change over time

**Structure:**

* IPv4 has **4 sections (octets)**

---

### 🔸 MAC Address (Physical Identity)

* Stands for: `Media Access Control`
* Unique hardware identifier
* Assigned at manufacturing
* Can be spoofed (security risk)

---

## Practical: MAC Address Spoofing

## Task 3:

Bypass network restriction by spoofing MAC address

### Concept:

* Network allowed only trusted MAC address
* Spoofing allowed unauthorized access

### Flag:

`THM{YOU_GOT_ON_TRYHACKME}`

---

## IP Address Concepts

* Each section of IP address is called: `Octet`
* IPv4 has: `4` octets
* Public IP → Internet communication
* Private IP → Internal network communication

---

## Ping & ICMP

## Task 4:

### 🔹 What is Ping?

Ping is a tool used to test connectivity between devices.

### 🔹 Protocol Used:

`ICMP (Internet Control Message Protocol)`

---

### 🔹 Syntax:

```id="code1"
ping 10.10.10.10
```

---

### Practical Task :

Pinged Google DNS:

```id="code2"
ping 8.8.8.8
```

### Flag:

`THM{I_PINGED_THE_SERVER}`

---

## Final Outcome

Successfully understood:

* Network fundamentals
* IP & MAC addressing
* Packet communication using ICMP
* Basic network security concept (MAC spoofing)

---

## Skills Gained

* Networking basics
* IP addressing knowledge
* MAC address concepts
* Using ping for connectivity testing
* Understanding spoofing attacks

---

## Real-World Relevance

This knowledge is essential for:

* Network Security
* Ethical Hacking
* SOC Analyst roles
* System Administration

---

## Challenges Faced

* Understanding difference between public & private IP
* Learning MAC spoofing concept

---


## Author

**Achal Deshmukh**

* 🎓 MCA Student
* 🔐 Cybersecurity Learner
* 📍 India

---

## ⭐ Notes

This room builds a strong foundation in networking, which is essential before moving into advanced cybersecurity topics like scanning, exploitation and defense.
