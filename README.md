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
