<div align="center">

# 💻 Introduction to Computer Systems (SWEN101)

## Group Assignment & Student Understanding Check

**Deadline: January 25, 2026**

---

</div>

## 📋 Course Information

| Field | Details |
|-------|---------|
| **Course Code** | SWEN101 |
| **Course Title** | Computer Systems |
| **Assignment Type** | Group Assignment |
| **Total Marks** | 100 |
| **Deadline** | January 25, 2026, 11:59 PM |

---

## ⚠️ IMPORTANT NOTICE

> **Note:** Some questions in this assignment may not have been fully addressed in the lectures so far. They are intentionally included to prepare you for upcoming topics and further study in Computer Systems. These questions require **critical thinking** and cannot be answered by simply copying from AI tools or textbooks.

---

## 📖 KEY DEFINITIONS

*These definitions apply to ALL scheduling questions in this assignment.*

| Term | Full Name | Formula/Definition |
|------|-----------|-------------------|
| **AT** | Arrival Time | Time when process enters ready queue |
| **BT** | Burst Time | Total CPU time required by process |
| **CT** | Completion Time | Time when process finishes execution |
| **TAT** | Turnaround Time | CT - AT |
| **WT** | Waiting Time | TAT - BT |
| **RT** | Response Time | Time of first CPU allocation - AT |

### 🔄 Tie-Breaking Rules

*Apply these rules to ALL scheduling questions:*

1. **Same Priority/Burst Time:** Use FCFS (earlier arrival time executes first)
2. **Same Arrival Time:** Use lower Process ID first (P1 before P2, P2 before P3, etc.)
3. **Round Robin Queue Order:** When a process arrives at the exact moment another completes its quantum, the arriving process joins the ready queue first

---

## 🎯 PART A: CPU SCHEDULING & OPERATING SYSTEM FUNDAMENTALS

### 🔢 Question 1 [25 Marks]

Suppose the following processes arrive for execution on a single CPU:

| **Process** | **Arrival Time (ms)** | **Burst Time (ms)** | **Priority** |
|:----------:|:--------------------:|:-------------------:|:------------:|
| **P1** | 0 | 8 | 2 |
| **P2** | 1 | 4 | 1 |
| **P3** | 2 | 9 | 3 |
| **P4** | 3 | 5 | 4 |
| **P5** | 4 | 2 | 5 |

> 📌 **Priority Convention:** Lower number = Higher priority (Priority 1 is the highest)

> 📌 **Tie-Breaking:** If processes have equal priority or burst time, use FCFS. If arrival times are also equal, prefer lower Process ID.

---

#### a) First Come First Serve (FCFS) [5 Marks]

**Required:**
- 📊 Draw the Gantt chart showing process execution order
- 🧮 Calculate CT, TAT, WT, RT for each process (use a table)
- 📈 Compute **Average Waiting Time (AWT)** and **Average Turnaround Time (ATAT)**

**Answer Template:**

| Process | AT | BT | CT | TAT | WT | RT |
|:-------:|:--:|:--:|:--:|:---:|:--:|:--:|
| P1 | 0 | 8 | | | | |
| P2 | 1 | 4 | | | | |
| P3 | 2 | 9 | | | | |
| P4 | 3 | 5 | | | | |
| P5 | 4 | 2 | | | | |
| **Average** | - | - | - | | | |

---

#### e) Priority Scheduling [5 Marks]

**Required:** Solve using **BOTH** methods:

##### e.1) Non-Preemptive Priority Scheduling [2.5 Marks]

> 📌 **Rule:** Once a process starts executing, it runs to completion regardless of new arrivals with higher priority.

| Process | AT | BT | Priority | CT | TAT | WT | RT |
|:-------:|:--:|:--:|:--------:|:--:|:---:|:--:|:--:|
| P1 | 0 | 8 | 2 | | | | |
| P2 | 1 | 4 | 1 | | | | |
| P3 | 2 | 9 | 3 | | | | |
| P4 | 3 | 5 | 4 | | | | |
| P5 | 4 | 2 | 5 | | | | |
| **Average** | - | - | - | - | | | |

##### e.2) Preemptive Priority Scheduling [2.5 Marks]

> 📌 **Preemption Rule:** A running process is preempted ONLY when a NEW process arrives with higher priority (lower priority number). The scheduler does not continuously check; it only evaluates at arrival times.

| Process | AT | BT | Priority | CT | TAT | WT | RT |
|:-------:|:--:|:--:|:--------:|:--:|:---:|:--:|:--:|
| P1 | 0 | 8 | 2 | | | | |
| P2 | 1 | 4 | 1 | | | | |
| P3 | 2 | 9 | 3 | | | | |
| P4 | 3 | 5 | 4 | | | | |
| P5 | 4 | 2 | 5 | | | | |
| **Average** | - | - | - | - | | | |

---

## 🔌 PART B: DIGITAL LOGIC & HARDWARE FUNDAMENTALS

### 🔢 Question 2 [15 Marks]

Seven switches (**S1, S2, S3, S4, S5, S6, S7**) control a lamp. The lamp turns **ON** (Output L = 1) when **ANY ONE** of the following conditions is satisfied:

| Condition | Switches that must be ON (= 1) | Switches that must be OFF (= 0) |
|:---------:|:------------------------------|:-------------------------------|
| 🟢 **Condition 1** | S1, S3, S5, S7 | S2 |
| 🟢 **Condition 2** | S2, S4, S6 | S3 |
| 🟢 **Condition 3** | S1, S2, S4, S6, S7 | *(none required OFF)* |

> 📌 **Important Notes:**
> - Switches not mentioned in a condition can be either ON or OFF (don't care for that condition)
> - The lamp turns ON if **at least one** condition is satisfied (OR relationship between conditions)
> - Convention: Switch ON = 1, Switch OFF = 0, Lamp ON = 1, Lamp OFF = 0

---

#### Task 1: Boolean Expression [5 Marks]

Write the Boolean expression for the lamp output **L** in terms of S1, S2, S3, S4, S5, S6, S7.

**Format your answer as:**

---

#### Task 2: Simplification [5 Marks]

Simplify the Boolean expression using Boolean algebra laws. 

**Show each step clearly with the law used:**

| Step | Expression | Law Applied |
|:----:|:-----------|:------------|
| 1 | *Original expression* | Given |
| 2 | | |
| 3 | | |
| ... | | |
| Final | *Simplified expression* | |

**Boolean Algebra Laws Reference:**
- Identity: A + 0 = A, A · 1 = A
- Null: A + 1 = 1, A · 0 = 0
- Idempotent: A + A = A, A · A = A
- Complement: A + A' = 1, A · A' = 0
- Commutative: A + B = B + A, A · B = B · A
- Associative: (A + B) + C = A + (B + C)
- Distributive: A · (B + C) = A·B + A·C, A + (B·C) = (A+B)·(A+C)
- Absorption: A + A·B = A, A·(A + B) = A
- De Morgan's: (A + B)' = A'·B', (A · B)' = A' + B'

---

#### Task 3: Logic Circuit [5 Marks]

Draw the logic circuit for the **simplified expression** using:
- AND gates (∧)
- OR gates (∨)  
- NOT gates (inverters)

**Requirements:**
- Label all inputs (S1-S7 as needed)
- Label the output (L)
- Use standard gate symbols
- Show all connections clearly

---

## 🏗️ PART C: COMPUTER ARCHITECTURE & SYSTEM ORGANIZATION

### 🔢 Question 3 [15 Marks]

Compare **Von Neumann Architecture** and **Harvard Architecture**.

---

#### a) Comparison Table [10 Marks]

Complete the following comparison table with detailed explanations:

| Aspect | Von Neumann Architecture | Harvard Architecture |
|:-------|:------------------------|:--------------------|
| **Memory Organization** | *Describe how memory is organized* | *Describe how memory is organized* |
| **Bus Structure** | *Describe the bus configuration* | *Describe the bus configuration* |
| **Instruction & Data Access** | *Can they be accessed simultaneously?* | *Can they be accessed simultaneously?* |
| **Speed/Performance** | *Relative performance and why* | *Relative performance and why* |
| **Cost & Complexity** | *Implementation cost and complexity* | *Implementation cost and complexity* |
| **Flexibility** | *How flexible is the design?* | *How flexible is the design?* |
| **Memory Utilization** | *How efficiently is memory used?* | *How efficiently is memory used?* |
| **Power Consumption** | *Relative power requirements* | *Relative power requirements* |

---

#### b) Advantages and Limitations [3 Marks]

**Von Neumann Architecture:**

| Advantages | Limitations |
|:-----------|:------------|
| 1. | 1. |
| 2. | 2. |

**Harvard Architecture:**

| Advantages | Limitations |
|:-----------|:------------|
| 1. | 1. |
| 2. | 2. |

---

#### c) Real-World Applications [2 Marks]

Provide **at least 2 specific examples** for each architecture and explain why that architecture is suitable.

**Von Neumann Applications:**

| Application | Why Von Neumann is Suitable |
|:------------|:---------------------------|
| 1. | |
| 2. | |

**Harvard Applications:**

| Application | Why Harvard is Suitable |
|:------------|:-----------------------|
| 1. | |
| 2. | |

---

## 🔢 PART D: BOOLEAN ALGEBRA & DIGITAL SYSTEMS

### 🔢 Question 4 [15 Marks]

Simplify the following Boolean function using a 4-variable Karnaugh Map:

$$F(A, B, C, D) = \prod M(0, 2, 5, 7, 8, 10, 13, 15)$$

> 📌 **Notation:** 
> - Π M denotes **Product of Sums (POS)** form
> - The numbers represent **maxterms** (combinations where F = 0)
> - Variable order: A is MSB, D is LSB (A B C D)

> 📌 **Maxterm Reference:**
> | Decimal | A | B | C | D |
> |:-------:|:-:|:-:|:-:|:-:|
> | 0 | 0 | 0 | 0 | 0 |
> | 2 | 0 | 0 | 1 | 0 |
> | 5 | 0 | 1 | 0 | 1 |
> | 7 | 0 | 1 | 1 | 1 |
> | 8 | 1 | 0 | 0 | 0 |
> | 10 | 1 | 0 | 1 | 0 |
> | 13 | 1 | 1 | 0 | 1 |
> | 15 | 1 | 1 | 1 | 1 |

---

#### Task 1: Construct K-Map [4 Marks]

Fill in the 4-variable K-map. Place **0** for maxterms and **1** for minterms.
                CD
          00    01    11    10
       +-----+-----+-----+-----+
AB  00 |     |     |     |     |
       +-----+-----+-----+-----+
    01 |     |     |     |     |
       +-----+-----+-----+-----+
    11 |     |     |     |     |
       +-----+-----+-----+-----+
    10 |     |     |     |     |
       +-----+-----+-----+-----+
       
---

#### Task 2: Group the Maxterms [4 Marks]

For POS simplification, group the **0s** (maxterms).

**Requirements:**
- Draw loops/circles around groups on the K-map
- Groups must be rectangular and contain 1, 2, 4, 8, or 16 cells
- Groups should be as large as possible
- Label each group (Group 1, Group 2, etc.)

**Show your grouped K-map here:**
                CD
          00    01    11    10
       +-----+-----+-----+-----+
AB  00 |     |     |     |     |
       +-----+-----+-----+-----+
    01 |     |     |     |     |
       +-----+-----+-----+-----+
    11 |     |     |     |     |
       +-----+-----+-----+-----+
    10 |     |     |     |     |
       +-----+-----+-----+-----+
       
**Groups identified:**
- Group 1: Cells ______, covers maxterms ______
- Group 2: Cells ______, covers maxterms ______
- (Add more if needed)

---

#### Task 3: Simplified POS Expression [4 Marks]

Derive the simplified POS expression from your groupings.

**Show your work:**

| Group | Cells Covered | Sum Term (Maxterm) |
|:-----:|:--------------|:-------------------|
| 1 | | |
| 2 | | |

**Final Simplified POS Expression:**

---

#### Task 4: Logic Circuit [3 Marks]

Draw the minimized logic circuit for your simplified POS expression.

**Requirements:**
- Use AND, OR, and NOT gates
- Label all inputs (A, B, C, D) and output (F)
- Use standard gate symbols

---

## 📚 PART E: CONCEPTUAL UNDERSTANDING [30 Marks]

*Answer the following questions concisely but completely. Each answer should be 50-150 words unless otherwise specified.*

---

### ❓ Question 5 [3 Marks]

**Why is CPU scheduling required in a multiprogramming system?**

List and explain at least **3 reasons**:

| # | Reason | Explanation |
|:-:|:-------|:------------|
| 1 | | |
| 2 | | |
| 3 | | |

---

### ❓ Question 6 [4 Marks]

**Differentiate between preemptive and non-preemptive scheduling.**

Complete the comparison table:

| Aspect | Preemptive Scheduling | Non-Preemptive Scheduling |
|:-------|:---------------------|:-------------------------|
| **Definition** | | |
| **Context Switching Frequency** | | |
| **Response Time** | | |
| **Starvation Risk** | | |
| **Implementation Complexity** | | |
| **Example Algorithm** | | |
| **Real-World Example** | | |

---

### ❓ Question 7 [4 Marks]

**Why does Shortest Job First (SJF) minimize average waiting time?**

**a) Explain the principle (1 mark):**

**b) Numerical Example (3 marks):**

Use these 3 processes to demonstrate:

| Process | Arrival Time | Burst Time |
|:-------:|:------------:|:----------:|
| P1 | 0 | 6 |
| P2 | 0 | 3 |
| P3 | 0 | 1 |

**Calculate Average WT using FCFS:**

**Comparison:** SJF reduces average WT by ______ ms (______%)

---

### ❓ Question 8 [4 Marks]

**How does time quantum affect the performance of Round Robin scheduling?**

Complete the analysis table:

| Time Quantum Size | Response Time | Throughput | Context Switch Overhead | Behavior |
|:------------------|:--------------|:-----------|:-----------------------|:---------|
| **Very Small** (e.g., 1 ms) | | | | |
| **Very Large** (e.g., 1000 ms) | | | | |
| **Optimal** | | | | |

**Recommended Time Quantum Range:** ______ to ______ ms

**Justification:**

---

### ❓ Question 9 [5 Marks]

**List the main components of the CPU and explain the function of each:**

| Component | Full Name | Primary Function | Specific Example of Operation |
|:----------|:----------|:-----------------|:-----------------------------|
| ⚙️ **CU** | Control Unit | | |
| ➕ **ALU** | Arithmetic Logic Unit | | |
| 📝 **Registers** | CPU Registers | | |
| 💾 **Cache** | Cache Memory | | |

---

### ❓ Question 10 [4 Marks]

**Explain the function of the following CPU registers:**

| Register | Full Name | What It Stores | When It Is Used | Example |
|:---------|:----------|:---------------|:----------------|:--------|
| ▶️ **PC** | Program Counter | | | |
| 🏠 **MAR** | Memory Address Register | | | |
| 💽 **MDR** | Memory Data Register | | | |
| 📋 **IR** | Instruction Register | | | |

---

### ❓ Question 11 [4 Marks]

**Describe the Instruction Execution Cycle (Fetch–Decode–Execute).**

#### a) Diagram [2 Marks]

Draw a flowchart or block diagram showing the instruction cycle. Include:
- All three stages
- Data flow between components
- Control signals

#### b) Stage Descriptions [2 Marks]

| Stage | What Happens | Registers/Components Involved |
|:------|:-------------|:-----------------------------|
| **Fetch** | | |
| **Decode** | | |
| **Execute** | | |

---

### ❓ Question 12 [4 Marks]

**Explain the Von Neumann Bottleneck.**

#### a) What causes this bottleneck? [1 Mark]

#### b) Why is it a significant limitation? [1 Mark]

#### c) Modern solutions [2 Marks]

List at least **3 techniques** modern systems use to address this bottleneck:

| # | Technique | How It Helps |
|:-:|:----------|:-------------|
| 1 | | |
| 2 | | |
| 3 | | |

---

## 💡 PART F: CRITICAL THINKING & REAL-WORLD APPLICATION [50 Marks]

> ⚠️ **Warning:** These questions require original thinking and analysis. Show your reasoning process clearly. AI-generated answers without proper analysis will receive zero marks.

---

### 🏥 Question 13 - Hospital Emergency Room Scheduling [12 Marks]

You are designing a scheduling algorithm for a hospital emergency room system.

**Patient Categories:**

| Severity Level | Description | Avg. Treatment Time | Maximum Acceptable Wait |
|:--------------|:------------|:-------------------|:-----------------------|
| 🔴 **CRITICAL** | Life-threatening | 30 minutes | Immediate (0 min) |
| 🟡 **URGENT** | Serious but stable | 20 minutes | 30 minutes |
| 🟢 **NORMAL** | Non-emergency | 15 minutes | 4 hours (240 min) |

**Arrival Pattern:** Average per hour: 2 CRITICAL, 5 URGENT, 15 NORMAL patients

---

#### a) Algorithm Selection [3 Marks]

**Which scheduling algorithm would you choose?**

**Your choice:** _______________________

**Comparison with alternatives:**

| Algorithm | Pros for This Scenario | Cons for This Scenario |
|:----------|:----------------------|:----------------------|
| Your Choice | | |
| Alternative 1 | | |
| Alternative 2 | | |

**Justification (consider patient safety, fairness, efficiency):**

---

#### b) Starvation Prevention [3 Marks]

**How would you prevent NORMAL patients from waiting indefinitely?**

**Proposed mechanism:**

**Specific thresholds:**
| Parameter | Value | Justification |
|:----------|:------|:--------------|
| Max wait before priority boost | | |
| Priority boost amount | | |
| Frequency of checking | | |

---

#### c) Tie-Breaking Mechanism [3 Marks]

**What happens when two CRITICAL patients arrive simultaneously?**

**Complete tie-breaking hierarchy:**

| Priority | Criterion | Reasoning |
|:---------|:----------|:----------|
| 1st | | |
| 2nd | | |
| 3rd | | |
| 4th | | |

---

#### d) Flowchart [3 Marks]

Draw a **detailed flowchart** showing your complete scheduling decision process.

**Must include:**
- Patient arrival and triage
- Priority assignment
- Starvation check
- Tie-breaking logic
- Treatment assignment

---

### 🅿️ Question 14 - Parking Lot Management System [12 Marks]

Design a parking lot management system with 4 floors.

**System Specifications:**
- Floor sensors: F1, F2, F3, F4 (F1 = ground floor, F4 = top floor)
- Sensor output: **1 = FULL**, **0 = AVAILABLE**
- Preference: Direct cars to lowest numbered available floor

---

#### a) Main Entrance FULL Indicator [2 Marks]

**Write the Boolean expression for the FULL indicator:**

The FULL sign illuminates (FULL = 1) when ALL floors are full.

---

#### b) Floor Selection Logic [4 Marks]

**Design floor selection using 2 output bits:**

| Selected Floor | Y1 | Y0 | Condition |
|:--------------|:--:|:--:|:----------|
| F1 (Ground) | 0 | 0 | F1 is available |
| F2 | 0 | 1 | F1 full, F2 available |
| F3 | 1 | 0 | F1,F2 full, F3 available |
| F4 (Top) | 1 | 1 | F1,F2,F3 full, F4 available |

**Boolean expressions:**

**Show your derivation:**

---

#### c) Complete Truth Table [2 Marks]

| F1 | F2 | F3 | F4 | FULL | Y1 | Y0 | Floor Selected |
|:--:|:--:|:--:|:--:|:----:|:--:|:--:|:--------------:|
| 0 | 0 | 0 | 0 | | | | |
| 0 | 0 | 0 | 1 | | | | |
| 0 | 0 | 1 | 0 | | | | |
| 0 | 0 | 1 | 1 | | | | |
| 0 | 1 | 0 | 0 | | | | |
| 0 | 1 | 0 | 1 | | | | |
| 0 | 1 | 1 | 0 | | | | |
| 0 | 1 | 1 | 1 | | | | |
| 1 | 0 | 0 | 0 | | | | |
| 1 | 0 | 0 | 1 | | | | |
| 1 | 0 | 1 | 0 | | | | |
| 1 | 0 | 1 | 1 | | | | |
| 1 | 1 | 0 | 0 | | | | |
| 1 | 1 | 0 | 1 | | | | |
| 1 | 1 | 1 | 0 | | | | |
| 1 | 1 | 1 | 1 | | | | |

---

#### d) Logic Circuit [2 Marks]

Draw the complete logic circuit for Y1 and Y0 outputs.

---

#### e) Capacity Tracking Enhancement [2 Marks]

If each floor has **50 parking spaces** and you need to track the **NUMBER of available spaces**:

| Question | Your Answer |
|:---------|:------------|
| What additional hardware is needed? | |
| How many bits to represent count per floor? | |
| How would the display system change? | |
| What type of circuits would replace simple sensors? | |

---

### 🚗 Question 15 - Self-Driving Car CPU Scheduling [12 Marks]

Design a CPU scheduling system for a self-driving car.

**Process Requirements:**

| **Process** | **Execution Time** | **Period/Deadline** | **Criticality** |
|:------------|:-----------------:|:------------------:|:---------------:|
| 🚨 Obstacle Detection | 5 ms | Deadline: 10 ms | CRITICAL |
| 🧭 Navigation Updates | 20 ms | Period: 100 ms | HIGH |
| 🎮 Entertainment System | 10-50 ms (variable) | Best effort | LOW |
| 🌡️ Climate Control | 10 ms | Period: 5000 ms | LOW |

> 📌 **Deadline** = Must complete within this time after trigger
> 📌 **Period** = Must run once every this interval

---

#### a) Real-Time Classification [2 Marks]

| Process | Classification | Justification |
|:--------|:--------------|:--------------|
| Obstacle Detection | ☐ Hard RT ☐ Soft RT ☐ Non-RT | |
| Navigation Updates | ☐ Hard RT ☐ Soft RT ☐ Non-RT | |
| Entertainment | ☐ Hard RT ☐ Soft RT ☐ Non-RT | |
| Climate Control | ☐ Hard RT ☐ Soft RT ☐ Non-RT | |

---

#### b) Algorithm Selection [3 Marks]

**Can a single algorithm handle all requirements?** ☐ Yes ☐ No

**Proposed scheduling approach:**

| Process Type | Algorithm Used | Why This Algorithm |
|:-------------|:---------------|:-------------------|
| Critical (Obstacle) | | |
| High Priority (Nav) | | |
| Low Priority (Ent/Climate) | | |

**How do the algorithms work together?**

---

#### c) Deadline Guarantee [2 Marks]

**Mechanisms to ensure critical processes NEVER miss deadlines:**

| Mechanism | Implementation | Effect |
|:----------|:--------------|:-------|
| CPU Reservation | | |
| Priority Level | | |
| Preemption Policy | | |

---

#### d) Graceful Degradation Strategy [3 Marks]

**When system becomes overloaded:**

| Overload Level | Action Taken | Processes Affected |
|:--------------|:-------------|:-------------------|
| Light (10% over) | | |
| Medium (25% over) | | |
| Severe (50%+ over) | | |

**Recovery procedure when load decreases:**

---

#### e) Timeline Diagram [2 Marks]

Draw a timeline showing process execution over **200 ms**.

**Assumptions:**
- Obstacle detection triggers at t=0, 50, 100, 150 ms
- Navigation runs at t=0, 100 ms
- Entertainment requests at t=30 ms (20 ms burst)
- Climate runs at t=0 ms

**Legend:** O = Obstacle, N = Navigation, E = Entertainment, C = Climate, I = Idle

---

### ⌨️ Question 16 - Keyboard to Screen Journey [8 Marks]

**Explain the complete journey of pressing the letter 'A' on your keyboard until it appears on your screen.**

---

#### Required Components [6 Marks]

| Component | Detailed Explanation |
|:----------|:--------------------|
| ⚡ **Hardware Interrupt** | How is the interrupt generated? What is the interrupt number? How does the CPU respond? What happens to the current process? |
| ⏱️ **CPU Scheduling** | What scheduling decisions are made? Which processes are involved (keyboard driver, OS, application)? Priority changes? |
| 💾 **Memory Operations** | What RAM read/write operations occur? Where is the keycode stored? How does it reach the application? |
| 📝 **Register Usage** | Which registers are used? What values do they hold? When are they loaded/stored? |
| 🚌 **Bus Communications** | What data travels on the data bus? What addresses on address bus? What control signals? |

---

#### Comprehensive Diagram [2 Marks]

Draw a diagram showing the complete flow including:
- Keyboard hardware
- Interrupt controller
- CPU (with registers)
- Memory
- Operating System
- Application
- Display output

---

### 📱 Question 17 - Architecture Selection for IoT Device [6 Marks]

**Scenario:** Design a temperature sensor IoT device with these requirements:
- 📊 Sample sensor data every 100 ms
- 🤖 Run simple anomaly detection algorithm
- 🔋 Operate on 2 AA batteries for 6+ months
- 💰 Total component cost under $5
- 💾 Store 24 hours of readings locally

---

#### Architecture Options Reference

| Architecture | Description |
|:-------------|:------------|
| **Von Neumann** | Single unified memory for instructions and data; single bus system |
| **Harvard** | Separate memories and buses for instructions and data |
| **Modified Harvard** | Separate caches but shared main memory; instructions can be read as data |

---

#### a) Architecture Comparison [4 Marks]

| Factor | Von Neumann | Harvard | Modified Harvard |
|:-------|:-----------:|:-------:|:----------------:|
| **Power Consumption** | | | |
| **Performance for This Task** | | | |
| **Implementation Cost** | | | |
| **Memory Efficiency** | | | |
| **Code Update Flexibility** | | | |
| **Suitability Score (1-5)** | | | |

---

#### b) Final Recommendation [2 Marks]

**Recommended Architecture:** _______________________

**Primary Justification:**

**Why not the other options:**

| Rejected Option | Reason for Rejection |
|:----------------|:--------------------|
| | |
| | |

---

## ⚖️ PART G: ETHICAL CONSIDERATIONS [15 Marks]

---

### 🏥 Question 18 - Medical Device Scheduling Ethics [6 Marks]

CPU scheduling decisions can have life-or-death implications in medical devices like pacemakers and insulin pumps.

---

#### a) Responsibility Analysis [2 Marks]

| Party | Responsibility Level (1-5) | Justification |
|:------|:------------------------:|:--------------|
| **Programmer** | | |
| **Company** | | |
| **Hospital** | | |
| **Regulatory Body (e.g., FDA)** | | |

**Who bears PRIMARY responsibility and why?**

---

#### b) Testing Strategies [2 Marks]

List at least **4 specific testing strategies** for a pacemaker's scheduling algorithm:

| # | Testing Strategy | Why It's Important |
|:-:|:-----------------|:-------------------|
| 1 | | |
| 2 | | |
| 3 | | |
| 4 | | |

---

#### c) Redundancy Measures [2 Marks]

Design a system with at least **3 layers of redundancy**:

| Layer | Redundancy Mechanism | What It Protects Against |
|:-----:|:--------------------|:------------------------|
| 1 | | |
| 2 | | |
| 3 | | |

---

### 🔄 Question 19 - Comparing Critical Systems [6 Marks]

Compare scheduling implementations across these four systems:

| Aspect | 🏧 ATM Machine | ✈️ Airplane Autopilot | 📱 Social Media App | ☢️ Nuclear Power Plant |
|:-------|:--------------|:---------------------|:-------------------|:----------------------|
| **Scheduling Algorithm** | | | | |
| **Priority Scheme** | | | | |
| **Failure Handling** | | | | |
| **Consequences of Delay** | | | | |
| **Real-Time Requirements** | | | | |
| **Redundancy Level** | | | | |

---

### 🎛️ Question 20 - Universal Gates Challenge [3 Marks]

You have **unlimited NAND gates only**.

---

#### a) XOR Implementation [1 Mark]

**Step 1: XOR Truth Table**

| A | B | A XOR B |
|:-:|:-:|:-------:|
| 0 | 0 | |
| 0 | 1 | |
| 1 | 0 | |
| 1 | 1 | |

**Step 2: Intermediate expressions**

Show how XOR can be expressed using AND, OR, NOT:

**Step 3: Convert to NAND-only**

Show substitutions:

**Step 4: Final circuit (must use exactly 4 NAND gates)**

---

#### b) Universal Gate Explanation [1 Mark]

**Why is NAND called a "universal gate"?**

**Demonstration:**

| Gate | NAND Implementation | Circuit |
|:-----|:-------------------|:--------|
| NOT | | |
| AND | | |
| OR | | |

---

#### c) Propagation Delay Calculation [1 Mark]

**Given:** Each NAND gate has 2 ns propagation delay

**Your XOR circuit's critical path:**

**Total propagation delay:** _______ ns

**Show your calculation:**

---

## 📤 SUBMISSION GUIDELINES

---

### 📋 Format Requirements

| Requirement | Specification |
|:------------|:-------------|
| **File Format** | PDF only (single file) |
| **File Naming** | `SWEN101_Group[X]_Assignment.pdf` |
| **Page Limit** | Maximum 35 pages (excluding cover page) |
| **Font** | Times New Roman, 12pt (text), 10pt (tables) |
| **Margins** | 1 inch (2.54 cm) on all sides |
| **Line Spacing** | 1.5 for text, single for tables |
| **Diagrams** | Minimum 300 DPI if scanned |

---

### ✅ Submission Checklist

Before submitting, verify:

- [ ] Cover page with all group member names and IDs
- [ ] Table of contents with page numbers
- [ ] All questions attempted (partial credit for incomplete answers)
- [ ] All calculations show complete step-by-step working
- [ ] All Gantt charts include clear time scale
- [ ] All diagrams are neat, labeled, and readable
- [ ] All truth tables are complete (no missing rows)
- [ ] All Boolean expressions clearly formatted
- [ ] All circuits use standard gate symbols
- [ ] Document spell-checked and proofread
- [ ] File size under 20 MB
- [ ] PDF is not password-protected

---

### 📊 Marking Rubric

| Criteria | Excellent (90-100%) | Good (70-89%) | Satisfactory (50-69%) | Needs Improvement (<50%) |
|:---------|:-------------------|:--------------|:---------------------|:------------------------|
| **Correctness** | All solutions mathematically correct | Minor calculation errors | Some significant errors | Major conceptual errors |
| **Working Shown** | Complete, clear, logical steps | Most steps shown clearly | Some steps missing/unclear | Little or no working |
| **Diagrams** | Professional, clear, properly labeled | Clear and labeled | Basic but understandable | Missing, unclear, or incorrect |
| **Critical Thinking** | Original, insightful, well-reasoned | Good analysis with evidence | Basic analysis attempted | No analysis or copied content |
| **Presentation** | Professional, well-organized | Good organization | Acceptable formatting | Poor organization, hard to follow |

---

### ⏰ Deadline & Penalties

| Item | Details |
|:-----|:--------|
| **Submission Deadline** | January 25, 2026, 11:59 PM (local time) |
| **Submission Portal** | [University LMS - Assignment Upload] |
| **Late Penalty** | -10% per day (including weekends) |
| **Maximum Late Period** | 5 days (after which: automatic 0) |
| **Technical Issues** | Email instructor BEFORE deadline with evidence |

---

### ⚠️ Academic Integrity

| Violation | Consequence |
|:----------|:------------|
| **Plagiarism** | Automatic ZERO for ALL group members |
| **AI-Generated Content** (without analysis) | ZERO for that question |
| **Copying from Other Groups** | ZERO for both groups |
| **Contract Cheating** | Reported to Academic Integrity Board |

---

### 👥 Group Members Declaration

| # | Full Name | Student ID | Email | Signature |
|:-:|:----------|:-----------|:------|:----------|
| 1 | | | | |
| 2 | | | | |
| 3 | | | | |

---

### 📜 Declaration Statement

> We, the undersigned members of this group, declare that:
> 1. This assignment is entirely our own original work
> 2. We have not copied from any source without proper citation
> 3. We have not used AI tools to generate answers without original analysis
> 4. We have not shared our work with other groups
> 5. All group members contributed fairly to this assignment

**Date:** _______________

**Group Number:** _______________

---

## 🏁 END OF ASSIGNMENT

---

<div align="center">

### Good Luck! 🍀

*If you have questions, contact me  during office hours or via email.*


</div>
