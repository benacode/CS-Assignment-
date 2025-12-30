<div align="center">

# 💻 Introduction to Computer Systems (SWEN101)

## Group Assignment & Student Understanding Check

### Academic Year 2025-2026

**Deadline: January 25, 2026, 11:59 PM**

---

![Computer Systems](https://img.shields.io/badge/Course-SWEN101-blue)
![Assignment](https://img.shields.io/badge/Type-Group%20Assignment-green)
![Marks](https://img.shields.io/badge/Total%20Marks-100-red)

</div>


## 📚 Course Information

| Field | Details |
|:------|:--------|
| **Course Code** | SWEN101 |
| **Course Title** | Introduction to Computer Systems |
| **Assignment Type** | Group Assignment |
| **Total Marks** | 100 |
| **Deadline** | January 25, 2026, 11:59 PM |
| **Submission Format** | PDF (Single File) |
| **Group Size** | 3 Members |

---

## ⚠️ IMPORTANT NOTICE

> **READ CAREFULLY BEFORE STARTING**
>
> Some questions in this assignment may not have been fully addressed in the lectures so far. They are intentionally included to:
> - Prepare you for upcoming topics
> - Encourage further study in Computer Systems
> - Develop critical thinking skills
>
> These questions **require original analysis** and cannot be answered by simply copying from AI tools or textbooks. Submissions that appear to be AI-generated without proper analysis will receive **zero marks**.

---

## 📖 KEY DEFINITIONS

*These definitions apply to ALL scheduling questions in this assignment.*

### Scheduling Metrics

| Term | Full Name | Formula/Definition |
|:-----|:----------|:-------------------|
| **AT** | Arrival Time | Time when process enters the ready queue |
| **BT** | Burst Time | Total CPU time required by the process |
| **CT** | Completion Time | Time when process finishes execution |
| **TAT** | Turnaround Time | CT - AT |
| **WT** | Waiting Time | TAT - BT |
| **RT** | Response Time | Time of first CPU allocation - AT |

### 🔄 Tie-Breaking Rules

*Apply these rules to ALL scheduling questions unless otherwise specified:*

| Priority | Rule | Description |
|:--------:|:-----|:------------|
| 1st | **FCFS** | Earlier arrival time executes first |
| 2nd | **Process ID** | Lower Process ID first (P1 before P2) |
| 3rd | **Round Robin Queue** | Arriving process joins queue before process completing quantum |


## 🎯 PART A: CPU SCHEDULING & OPERATING SYSTEM FUNDAMENTALS

### 🔢 **Question 1**

Suppose the following processes arrive for execution on a single CPU:

| **Process** | **Arrival Time** | **Burst Time** | **Priority** |
|------------|------------------|----------------|--------------|
| **P1**      | 0                | 8              | 2            |
| **P2**      | 1                | 4              | 1            |
| **P3**      | 2                | 9              | 3            |
| **P4**      | 3                | 5              | 4            |
| **P5**      | 4                | 2              | 5            |

> 📌 *Lower number = Higher priority*

Solve using the following scheduling algorithms:

#### **a) First Come First Serve (FCFS)**
- 📊 Draw the Gantt chart
- 🧮 Calculate CT, TAT, WT, RT for each process
- 📈 Compute Average Waiting Time

#### **b) Shortest Job First (SJF – Non-Preemptive)**
- 📊 Draw the Gantt chart
- 🧮 Calculate CT, TAT, WT, RT for each process

#### **c) Shortest Remaining Time First (SRTF – Preemptive)**
- 📊 Draw the Gantt chart
- 🧮 Calculate CT, TAT, WT, RT for each process

#### **d) Round Robin Scheduling (Time Quantum = 4 ms)**
- 📊 Draw the Gantt chart
- 🧮 Calculate CT, TAT, WT, RT for each process

#### **e) Priority Scheduling**
- 🔄 Solve using both Preemptive and Non-Preemptive methods
- 📊 Draw Gantt charts and compute all timing metrics

**Where:**
- **CT** = Completion Time
- **TAT** = Turnaround Time
- **WT** = Waiting Time
- **RT** = Response Time



## 🔌 PART B: DIGITAL LOGIC & HARDWARE FUNDAMENTALS

### 🔢 **Question 2**

Seven switches (**S1, S2, S3, S4, S5, S6, S7**) operate a lamp under the following conditions:

- 🟢 **Condition 1:** Switches 1, 3, 5, and 7 are ON and switch 2 is OFF
- 🟢 **Condition 2:** Switches 2, 4, and 6 are ON and switch 3 is OFF
- 🟢 **Condition 3:** All switches are ON

#### **Tasks:**
1. ✍️ Write the Boolean expression for the lamp output
2. 🔧 Simplify the expression using Boolean algebra laws
3. 🛠️ Draw the logic circuit using AND, OR, and NOT gates



## 🏗️ PART C: COMPUTER ARCHITECTURE & SYSTEM ORGANIZATION

### 🔢 **Question 3**

Compare **Von Neumann** and **Harvard Architectures** in terms of:
- 🧠 Memory organization
- 🚌 Bus structure
- ⚡ Performance characteristics
- ✅ Advantages and limitations
- 🌍 Real-world applications (provide specific examples)



## 🔢 PART D: BOOLEAN ALGEBRA & DIGITAL SYSTEMS

### 🔢 **Question 4**
Simplify the following Boolean function using a 4-variable Karnaugh Map:

$$\Large F(A, B, C, D) = \prod M(0, 2, 5, 7, 8, 10, 13, 15)$$

> 📌 **Notation:** 
> - **Π M** denotes **Product of Sums (POS)** form
> - The numbers represent **maxterms** (combinations where F = 0)
> - Variable order: **A** is MSB, **D** is LSB

**Maxterm Reference Table:**

| Decimal | A | B | C | D | F (0 = maxterm) |
|:-------:|:-:|:-:|:-:|:-:|:---------------:|
| 0 | 0 | 0 | 0 | 0 | 0 |
| 1 | 0 | 0 | 0 | 1 | 1 |
| 2 | 0 | 0 | 1 | 0 | 0 |
| 3 | 0 | 0 | 1 | 1 | 1 |
| 4 | 0 | 1 | 0 | 0 | 1 |
| 5 | 0 | 1 | 0 | 1 | 0 |
| 6 | 0 | 1 | 1 | 0 | 1 |
| 7 | 0 | 1 | 1 | 1 | 0 |
| 8 | 1 | 0 | 0 | 0 | 0 |
| 9 | 1 | 0 | 0 | 1 | 1 |
| 10 | 1 | 0 | 1 | 0 | 0 |
| 11 | 1 | 0 | 1 | 1 | 1 |
| 12 | 1 | 1 | 0 | 0 | 1 |
| 13 | 1 | 1 | 0 | 1 | 0 |
| 14 | 1 | 1 | 1 | 0 | 1 |
| 15 | 1 | 1 | 1 | 1 | 0 |

#### **Tasks:**
1. 🗺️ Construct the K-map for POS (Product of Sums)
2. 👥 Group the maxterms appropriately
3. ✨ Obtain the simplified POS expression
4. 🛠️ Draw the minimized logic circuit



## 📚 PART E: CONCEPTUAL UNDERSTANDING

*Answer the following questions concisely but completely:*

#### ❓ **Question 5**
Why is CPU scheduling required in a multiprogramming system?

#### ❓ **Question 6**
Differentiate between preemptive and non-preemptive scheduling. Provide one example of each.

#### ❓ **Question 7**
Why does Shortest Job First (SJF) minimize average waiting time? Explain with a simple example.

#### ❓ **Question 8**
How does time quantum affect the performance of Round Robin scheduling? Discuss what happens with very small and very large quantum values.

#### ❓ **Question 9**
List the main components of the CPU and explain the function of each:
- ⚙️ Control Unit (CU)
- ➕ Arithmetic Logic Unit (ALU)
- 📝 Registers
- 💾 Cache

#### ❓ **Question 10**
Explain the function of the following CPU registers:
- ▶️ Program Counter (PC)
- 🏠 Memory Address Register (MAR)
- 💽 Memory Data Register (MDR)
- 📋 Instruction Register (IR)

#### ❓ **Question 11**
Describe the instruction execution cycle (**Fetch–Decode–Execute**) with a diagram. What happens at each stage?

#### ❓ **Question 12**
Explain the **Von Neumann bottleneck**. Why is it a limitation and how do modern systems address it?



## 💡 PART F: CRITICAL THINKING & REAL-WORLD APPLICATION

*These questions require original thinking and analysis. Show your reasoning process clearly.*

### 🏥 **Question 13 - Hospital Emergency Room Scheduling**

You are designing a scheduling algorithm for a hospital emergency room system where patients arrive with different severity levels:
- 🔴 **CRITICAL** (life-threatening)
- 🟡 **URGENT** (serious but stable)
- 🟢 **NORMAL** (non-emergency)

#### **Answer the following:**

**a)** Which scheduling algorithm would you choose and why? Justify your selection over other alternatives.

**b)** How would you modify the algorithm to prevent starvation of normal patients who might wait indefinitely?

**c)** What happens if two critical patients arrive simultaneously? Design a tie-breaking mechanism.

**d)** Draw a flowchart showing your complete scheduling decision process.



### 🅿️ **Question 14 - Parking Lot Management System**

Design a parking lot management system with 4 floors where:
- Each floor has a sensor indicating **FULL (1)** or **AVAILABLE (0)**
- Floor sensors are labeled: **F1, F2, F3, F4**
- The entrance display should show **"FULL"** only when ALL floors are full
- The system should direct cars to the nearest available floor

#### **Tasks:**

**a)** Write the Boolean expression for the main entrance "FULL" indicator

**b)** Design the floor selection logic that outputs which floor a car should go to (prefer lower floors when multiple are available)

**c)** Create a truth table for 4 floors showing all 16 combinations

**d)** Draw the complete logic circuit

**e)** What modifications would you make if the system needed to track the **NUMBER** of available spaces on each floor?



### 🚗 **Question 15 - Self-Driving Car CPU Scheduling**

Design a CPU scheduling system for a self-driving car that must handle the following processes:

| **Process** | **Response Required** | **Priority** |
|-------------|----------------------|--------------|
| 🚨 Obstacle Detection | Within 10ms | CRITICAL |
| 🧭 Navigation Updates | Every 100ms | HIGH |
| 🎮 Entertainment | Best effort | LOW |
| 🌡️ Climate Control | Every 5 seconds | LOW |

#### **Answer the following:**

**a)** Classify which processes are real-time vs non-real-time. Explain why.

**b)** What scheduling algorithm(s) would you use? Can a single algorithm handle all requirements?

**c)** How do you ensure critical processes **NEVER** miss their deadlines?

**d)** What happens if the system becomes overloaded? Design a graceful degradation strategy.

**e)** Draw a timeline showing how your scheduler would handle all four processes over a 1-second period.



### ⌨️ **Question 16 - Keyboard to Screen Journey**

Explain the complete journey of pressing the letter 'A' on your keyboard until it appears on your screen. Your explanation must include:

- ⚡ Hardware interrupt generation and handling
- ⏱️ CPU scheduling decisions made
- 💾 Memory operations (RAM access)
- 📝 Register usage (which registers are involved)
- 🚌 Bus communications (data flow)

**Draw a diagram showing this complete flow.**



### 📱 **Question 17 - Architecture Selection for IoT Device**

Your company is designing a new IoT device with these requirements:
- 📊 Process sensor data in real-time
- 🤖 Run simple machine learning inference
- 🔋 Operate on battery power for 6 months
- 💰 Cost less than $5 per unit

Which architecture would you choose: **Von Neumann, Harvard, or Modified Harvard?**

#### **Justify your decision considering:**
**a)** Power consumption implications  
**b)** Performance requirements  
**c)** Cost constraints  
**d)** Memory efficiency  

**Compare at least TWO architectures before making your final recommendation.**



## ⚖️ PART G: ETHICAL CONSIDERATIONS

### 🏥 **Question 18 - Medical Device Scheduling Ethics**

CPU scheduling decisions can have life-or-death implications in medical devices like pacemakers and insulin pumps.

**a)** Who should be held responsible if a scheduling bug causes patient harm: the programmer, the company, the hospital, or the regulatory body?

**b)** How would you test a pacemaker's scheduling algorithm before deployment? What testing strategies would you use?

**c)** What redundancy measures would you implement to prevent scheduling failures in a life-critical medical device?



### 🔄 **Question 19 - Comparing Critical Systems**

Compare how the following four systems would implement process scheduling differently:

1. 🏧 **ATM Machine**
2. ✈️ **Airplane Autopilot System**
3. 📱 **Social Media Mobile App**
4. ☢️ **Nuclear Power Plant Control System**

#### **For EACH system, identify:**
- 🔧 Type of scheduling algorithm most suitable
- ⭐ Priority considerations
- 🛡️ Failure handling mechanisms
- ⏰ Consequences of scheduling delays



### 🎛️ **Question 20 - Universal Gates Challenge**

You have unlimited **NAND gates** only.

**a)** Show step-by-step how you would implement a 2-input XOR gate using only NAND gates. Draw the circuit.

**b)** Explain why NAND is called a "universal gate"

**c)** What is the minimum number of NAND gates required to implement XOR?

**d)** What is the propagation delay of your XOR circuit if each NAND gate has a 2ns delay?



### ✅ Pre-Submission Checklist

**Content Completeness:**
- [ ] All questions from Part A to Part G attempted
- [ ] All Gantt charts include time scale and process labels
- [ ] All calculations show step-by-step working
- [ ] All truth tables are complete (no missing rows)
- [ ] All Boolean expressions are clearly formatted
- [ ] All logic circuits use standard gate symbols
- [ ] All diagrams are labeled and referenced in text

**Formatting:**
- [ ] Cover page with all required information
- [ ] Table of contents with page numbers
- [ ] Questions numbered clearly matching this document
- [ ] Consistent formatting throughout
- [ ] Page numbers on all pages
- [ ] Readable font size (not smaller than 10pt)

**Quality Checks:**
- [ ] Spelling and grammar checked
- [ ] All diagrams are clear and legible
- [ ] Mathematical notation is correct
- [ ] References cited if external sources used
- [ ] File opens correctly in PDF reader

**Technical:**
- [ ] File is in PDF format
- [ ] File name follows naming convention
- [ ] File size under 25 MB
- [ ] PDF is not password-protected
- [ ] All pages are properly oriented

---

### 📊 Marking Rubric

| Criteria | Excellent (90-100%) | Good (70-89%) | Satisfactory (50-69%) | Needs Improvement (<50%) |
|:---------|:-------------------|:--------------|:---------------------|:------------------------|
| **Correctness** | All solutions mathematically/logically correct | Minor calculation or logical errors | Some significant errors | Major conceptual errors |
| **Working Shown** | Complete, clear, logical steps for all problems | Most steps shown clearly | Some steps missing or unclear | Little or no working shown |
| **Diagrams/Charts** | Professional, clear, properly labeled, accurate | Clear and labeled with minor issues | Basic but understandable | Missing, unclear, or incorrect |
| **Critical Thinking** | Original, insightful, well-reasoned analysis | Good analysis with evidence | Basic analysis attempted | No analysis or copied content |
| **Completeness** | All questions fully answered | Most questions fully answered | Some questions incomplete | Many questions missing |
| **Presentation** | Professional, well-organized, easy to follow | Good organization | Acceptable formatting | Poor organization |

---

### ⏰ Deadline and Late Submission Policy

| Item | Details |
|:-----|:--------|
| **Submission Deadline** | January 25, 2026, 11:59 PM (Local Time) |
| **Submission Portal** | University LMS → SWEN101 → Assignments |
| **Late Penalty** | -10% per day (including weekends and holidays) |
| **Maximum Late Period** | 5 days |
| **After 5 Days Late** | Automatic 0% |
| **Technical Issues** | Email instructor BEFORE deadline with evidence |
| **Extension Requests** | Submit in writing at least 48 hours before deadline |

**Late Submission Calculation:**

| Days Late | Maximum Possible Score |
|:---------:|:----------------------:|
| 0 (On time) | 100% |
| 1 | 90% |
| 2 | 80% |
| 3 | 70% |
| 4 | 60% |
| 5 | 50% |
| 6+ | 0% |

---

### ⚠️ Academic Integrity Policy

| Violation | First Offense | Repeat Offense |
|:----------|:-------------|:---------------|
| **Plagiarism** | 0% for assignment + warning | Course failure + disciplinary hearing |
| **AI-Generated Content** (without analysis) | 0% for that question | 0% for assignment |
| **Copying from Other Groups** | 0% for BOTH groups | Course failure for all involved |
| **Contract Cheating** | Course failure | Expulsion proceedings |
| **Unauthorized Collaboration** | 0% for assignment | Course failure |

**What is Allowed:**
- ✅ Discussing concepts with classmates
- ✅ Using lecture notes and textbooks
- ✅ Referencing online resources (with citation)
- ✅ Using AI tools to understand concepts (not to generate answers)

**What is NOT Allowed:**
- ❌ Copying solutions from any source
- ❌ Sharing your solutions with other groups
- ❌ Using AI to generate answers directly
- ❌ Submitting work done by others
- ❌ Purchasing or selling assignment solutions

---

### 👥 Group Member Declaration

**Group Number:** _______________

| # | Full Name | Student ID | Email Address | Contribution (%) | Signature |
|:-:|:----------|:-----------|:--------------|:----------------:|:---------:|
| 1 | | | | | |
| 2 | | | | | |
| 3 | | | | | |

**Total Contribution Must Equal 100%**

---

### 📜 Honor Code Statement

> **We, the undersigned members of this group, solemnly declare that:**
>
> 1. This assignment represents our own original work
> 2. We have not copied solutions from any unauthorized source
> 3. We have not shared our solutions with any other group
> 4. We have not used AI tools to generate answers without proper analysis
> 5. All external sources have been properly cited
> 6. We have contributed fairly to this assignment as indicated above
> 7. We understand and accept the academic integrity policy
> 8. We accept responsibility for any violations discovered
>
> **We acknowledge that any violation of academic integrity will result in disciplinary action as outlined in the university's academic integrity policy.**

**Signatures:**

| Member | Signature | Date |
|:-------|:----------|:-----|
| Member 1 | | |
| Member 2 | | |
| Member 3 | | |

---

## 🏁 END OF ASSIGNMENT

---

<div align="center">

### 🍀 Good Luck!

*If you have questions, contact me during office hours or via email.*


*This assignment was designed to test your understanding of computer systems concepts and your ability to apply them to real-world scenarios. Take your time, think critically, and show your work!*
</div>



## 🏁 END OF ASSIGNMENT
