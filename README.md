# BITS COLLEGE
## SCHOOL OF SYSTEMS AND TECHNOLOGY
### Introduction to Computer Systems (SWEN101)

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

**SWEN101: Computer Systems**  
**Group Assignment & Student Understanding Check**

**Deadline: January 25, 2025**

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

### IMPORTANT NOTICE:
Some questions in this assignment may not have been fully addressed in the lectures so far. They are intentionally included to prepare you for upcoming topics and further study in Computer Systems. These questions require critical thinking and cannot be answered by simply copying from AI tools or textbooks.

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

## PART A: CPU SCHEDULING & OPERATING SYSTEM FUNDAMENTALS

### Question 1

Suppose the following processes arrive for execution on a single CPU:

| Process | Arrival Time | Burst Time | Priority |
|---------|--------------|------------|----------|
| P1      | 0            | 8          | 2        |
| P2      | 1            | 4          | 1        |
| P3      | 2            | 9          | 3        |
| P4      | 3            | 5          | 4        |
| P5      | 4            | 2          | 5        |

*(Lower number = Higher priority)*

Solve using the following scheduling algorithms:

**a) First Come First Serve (FCFS)**
- Draw the Gantt chart
- Calculate CT, TAT, WT, RT for each process
- Compute Average Waiting Time

**b) Shortest Job First (SJF – Non-Preemptive)**
- Draw the Gantt chart
- Calculate CT, TAT, WT, RT for each process

**c) Shortest Remaining Time First (SRTF – Preemptive)**
- Draw the Gantt chart
- Calculate CT, TAT, WT, RT for each process

**d) Round Robin Scheduling (Time Quantum = 4 ms)**
- Draw the Gantt chart
- Calculate CT, TAT, WT, RT for each process

**e) Priority Scheduling**
- Solve using both Preemptive and Non-Preemptive methods
- Draw Gantt charts and compute all timing metrics

*Where:*
- CT = Completion Time
- TAT = Turnaround Time
- WT = Waiting Time
- RT = Response Time

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

## PART B: DIGITAL LOGIC & HARDWARE FUNDAMENTALS

### Question 2

Seven switches (S1, S2, S3, S4, S5, S6, S7) operate a lamp under the following conditions:

- **Condition 1:** Switches 1, 3, 5, and 7 are ON and switch 2 is OFF
- **Condition 2:** Switches 2, 4, and 6 are ON and switch 3 is OFF
- **Condition 3:** All switches are ON

**Tasks:**
1. Write the Boolean expression for the lamp output
2. Simplify the expression using Boolean algebra laws
3. Draw the logic circuit using AND, OR, and NOT gates

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

## PART C: COMPUTER ARCHITECTURE & SYSTEM ORGANIZATION

### Question 3

Compare Von Neumann and Harvard Architectures in terms of:
- Memory organization
- Bus structure
- Performance characteristics
- Advantages and limitations
- Real-world applications (provide specific examples)

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

## PART D: BOOLEAN ALGEBRA & DIGITAL SYSTEMS

### Question 4

Simplify the Boolean function using a 4-variable Karnaugh Map:

**Tasks:**
1. Construct the K-map for POS (Product of Sums)
2. Group the maxterms appropriately
3. Obtain the simplified POS expression
4. Draw the minimized logic circuit

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

## PART E: CONCEPTUAL UNDERSTANDING

*Answer the following questions concisely but completely:*

### Question 5
Why is CPU scheduling required in a multiprogramming system?

### Question 6
Differentiate between preemptive and non-preemptive scheduling. Provide one example of each.

### Question 7
Why does Shortest Job First (SJF) minimize average waiting time? Explain with a simple example.

### Question 8
How does time quantum affect the performance of Round Robin scheduling? Discuss what happens with very small and very large quantum values.

### Question 9
List the main components of the CPU and explain the function of each:
- Control Unit (CU)
- Arithmetic Logic Unit (ALU)
- Registers
- Cache

### Question 10
Explain the function of the following CPU registers:
- Program Counter (PC)
- Memory Address Register (MAR)
- Memory Data Register (MDR)
- Instruction Register (IR)

### Question 11
Describe the instruction execution cycle (Fetch–Decode–Execute) with a diagram. What happens at each stage?

### Question 12
Explain the Von Neumann bottleneck. Why is it a limitation and how do modern systems address it?

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

## PART F: CRITICAL THINKING & REAL-WORLD APPLICATION

*These questions require original thinking and analysis. Show your reasoning process clearly.*

### Question 13 - Hospital Emergency Room Scheduling

You are designing a scheduling algorithm for a hospital emergency room system where patients arrive with different severity levels:
- **CRITICAL** (life-threatening)
- **URGENT** (serious but stable)
- **NORMAL** (non-emergency)

**Answer the following:**

a) Which scheduling algorithm would you choose and why? Justify your selection over other alternatives.

b) How would you modify the algorithm to prevent starvation of normal patients who might wait indefinitely?

c) What happens if two critical patients arrive simultaneously? Design a tie-breaking mechanism.

d) Draw a flowchart showing your complete scheduling decision process.

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

### Question 14 - Parking Lot Management System

Design a parking lot management system with 4 floors where:
- Each floor has a sensor indicating FULL (1) or AVAILABLE (0)
- Floor sensors are labeled: F1, F2, F3, F4
- The entrance display should show "FULL" only when ALL floors are full
- The system should direct cars to the nearest available floor

**Tasks:**

a) Write the Boolean expression for the main entrance "FULL" indicator

b) Design the floor selection logic that outputs which floor a car should go to (prefer lower floors when multiple are available)

c) Create a truth table for 4 floors showing all 16 combinations

d) Draw the complete logic circuit

e) What modifications would you make if the system needed to track the NUMBER of available spaces on each floor?

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

### Question 15 - Self-Driving Car CPU Scheduling

Design a CPU scheduling system for a self-driving car that must handle the following processes:

| Process | Response Required | Priority |
|---------|-------------------|----------|
| Obstacle Detection | Within 10ms | CRITICAL |
| Navigation Updates | Every 100ms | HIGH |
| Entertainment | Best effort | LOW |
| Climate Control | Every 5 seconds | LOW |

**Answer the following:**

a) Classify which processes are real-time vs non-real-time. Explain why.

b) What scheduling algorithm(s) would you use? Can a single algorithm handle all requirements?

c) How do you ensure critical processes NEVER miss their deadlines?

d) What happens if the system becomes overloaded? Design a graceful degradation strategy.

e) Draw a timeline showing how your scheduler would handle all four processes over a 1-second period.

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

### Question 16 - Keyboard to Screen Journey

Explain the complete journey of pressing the letter 'A' on your keyboard until it appears on your screen. Your explanation must include:

- Hardware interrupt generation and handling
- CPU scheduling decisions made
- Memory operations (RAM access)
- Register usage (which registers are involved)
- Bus communications (data flow)

Draw a diagram showing this complete flow.

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

### Question 17 - Architecture Selection for IoT Device

Your company is designing a new IoT device with these requirements:
- Process sensor data in real-time
- Run simple machine learning inference
- Operate on battery power for 6 months
- Cost less than $5 per unit

Which architecture would you choose: Von Neumann, Harvard, or Modified Harvard?

**Justify your decision considering:**
a) Power consumption implications
b) Performance requirements
c) Cost constraints
d) Memory efficiency

Compare at least TWO architectures before making your final recommendation.

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

## PART G: ETHICAL CONSIDERATIONS

### Question 18 - Medical Device Scheduling Ethics

CPU scheduling decisions can have life-or-death implications in medical devices like pacemakers and insulin pumps.

a) Who should be held responsible if a scheduling bug causes patient harm: the programmer, the company, the hospital, or the regulatory body?

b) How would you test a pacemaker's scheduling algorithm before deployment? What testing strategies would you use?

c) What redundancy measures would you implement to prevent scheduling failures in a life-critical medical device?

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

### Question 19 - Comparing Critical Systems

Compare how the following four systems would implement process scheduling differently:

1. ATM Machine
2. Airplane Autopilot System
3. Social Media Mobile App
4. Nuclear Power Plant Control System

**For EACH system, identify:**
- Type of scheduling algorithm most suitable
- Priority considerations
- Failure handling mechanisms
- Consequences of scheduling delays

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

### Question 20 - Universal Gates Challenge

You have unlimited NAND gates only.

a) Show step-by-step how you would implement a 2-input XOR gate using only NAND gates. Draw the circuit.

b) Explain why NAND is called a "universal gate"

c) What is the minimum number of NAND gates required to implement XOR?

d) What is the propagation delay of your XOR circuit if each NAND gate has a 2ns delay?

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

## SUBMISSION GUIDELINES

- Submit as a GROUP with all member names clearly listed
- Show all working for calculation questions
- Diagrams must be neat and clearly labeled
- Critical thinking questions require YOUR OWN analysis - AI-generated answers will be penalized
- Late submissions: -10% per day
- Plagiarism will result in automatic ZERO for all group members

**Group Members:**

1. ____________________________ ID: ________________
2. ____________________________ ID: ________________
3. ____________________________ ID: ________________
4. ____________________________ ID: ________________
5. ____________________________ ID: ________________

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

## END OF ASSIGNMENT