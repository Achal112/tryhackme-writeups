# Computer Fundamentals – TryHackMe Write-up

## Room Information

* **Platform:** TryHackMe
* **Module:** Computer Fundamentals
* **Room Name:** Computer Fundamentals
* **Difficulty:** Beginner
* **Status:** ✅ Completed

---

# Objective

Learn:

* Basic computer components
* How a computer starts (boot process)
* Functions of different hardware parts

---

# Task 1: Introduction

### 🔹 Concept

Before securing a computer system, we must first understand:

* What a computer is
* How components work together
* How systems start and operate

The room compares a computer system to a castle:

> You cannot defend something properly if you don’t understand it first.

---

### ✅ Answer:

* No answer required

---

# Task 2: Inside a Computer System

### 🔹 Core Components Learned

| Component   | Function               |
| ----------- | ---------------------- |
| CPU         | Processes instructions |
| RAM         | Temporary memory       |
| Storage     | Saves files and OS     |
| Motherboard | Connects components    |
| PSU         | Supplies power         |
| GPU         | Handles graphics       |

---

### 🔹 Important Point

All components work together to make the computer functional.

---

### Practical Activity

Completed interactive component identification exercise.

---

### ✅ Flag:

```bash id="i1q0x4"
THM{4llpccomp0n3nts1d3nt1f13d}
```

---

# Task 3: What Happens When You Press the Start Button?

### 🔹 Boot Process Steps

## 1. Power Button Pressed

* PSU starts supplying electricity.

---

## 2. Firmware Starts

* UEFI/BIOS initializes hardware.

---

## 3. Power-On Self Test (POST)

* System checks if components work correctly.

---

## 4. Boot Device Selection

* System searches for operating system.

---

## 5. Bootloader Starts

* OS loads into RAM and starts.

---

### 🔹 Important Terms

* **UEFI/BIOS** → Firmware
* **POST** → Hardware checking process
* **Bootloader** → Loads operating system

---

### Practical Activity

Completed boot sequence simulation exercise.

---

### ✅ Flag:

```bash id="v8d9tm"
THM{pc5ucce55fully5t4rt3d}
```

---

# Task 4: Conclusion

### 🔹 Summary

Learned:

* Internal computer components
* Boot sequence
* Hardware interactions

These concepts are important because attackers often target:

* Boot process
* Firmware
* Hardware components

---

### ✅ Answer:

* No answer required

---

# Skills Gained

* Basic computer architecture knowledge
* Understanding system startup process
* Hardware component identification

---

# Real-World Relevance

Useful for:

* Cybersecurity
* System Administration
* IT Support
* Ethical Hacking

---

# Challenges Faced

* Understanding firmware and boot process
* Learning hardware component roles

---

# Author

**Achal Deshmukh**

* 🎓 MCA Student
* 🔐 Cybersecurity Learner

---

# ⭐ Notes

Understanding how computers work internally is the foundation for learning cybersecurity, networking, and operating systems.
