# Assignment Questions

## Instructions
Answer all 4 questions with detailed explanations. Each answer should be **3-5 sentences minimum** and demonstrate your understanding of the concepts.

---

## Question 1: Thread vs Process

**Question**: Explain the difference between a **thread** and a **process**. Why did we use threads in this assignment instead of creating separate processes?

**Your Answer:**

[A process is an independent program with its own memory space, while a thread is a smaller unit of execution within a process that shares the same memory. Threads are lighter and faster to create compared to processes. In this assignment, we used threads because they allow multiple tasks to run concurrently within the same program. This improves performance and resource usage. Using processes would be more complex and slower due to separate memory spaces.]

---

## Question 2: Ready Queue Behavior

**Question**: In Round-Robin scheduling, what happens when a process doesn't finish within its time quantum? Explain using an example from your program output.

**Your Answer:**

In Round-Robin scheduling, if a process does not finish within its time quantum, it is placed back at the end of the ready queue. This means it will wait for its next turn while other processes get CPU time. For example, if process P1 has a burst time longer than the time quantum, it will run for a limited time and then be paused. After that, it is re-queued and will continue execution later. This ensures fairness among all processes.

Example from my output:
P1 is running for 2 units
P1 did not finish and is moved to the end of the queue

Explanation of example:
In this example, P1 used its allocated time quantum but did not complete its execution. Therefore, it was returned to the ready queue. Later, it will be scheduled again and continue from where it left off. This behavior ensures that no single process monopolizes the CPU.
```

---

## Question 3: Thread States

**Question**: A thread can be in different states: **New**, **Runnable**, **Running**, **Waiting**, **Terminated**. Walk through these states for one process (P1) from your simulation.

**Your Answer:**

[]

1. **New**: [When is P1 in New state?P1 is in the New state when it is first created but has not started execution yet.]

2. **Runnable**: [When does P1 become Runnable?P1 becomes Runnable when it is added to the ready queue and is waiting for CPU time.]

3. **Running**: [When is P1 Running?P1 is in the Running state when the scheduler selects it and assigns CPU time to execute.]

4. **Waiting**: [When/why would P1 be Waiting?P1 may enter the Waiting state if it is paused or waiting for its next turn after its time quantum expires.]

5. **Terminated**: [When is P1 Terminated?P1 reaches the Terminated state when it finishes execution completely and no longer needs CPU time.]

---

## Question 4: Real-World Applications

**Question**: Give **TWO** real-world examples where Round-Robin scheduling with threads would be useful. Explain why this scheduling algorithm works well for those scenarios.

**Your Answer:**

### Example 1: [Web Server]

**Description**: 
[A web server handles multiple client requests at the same time. Each request can be processed as a separate thread.]

**Why Round-Robin works well here**: 
[Round-Robin ensures that each client request gets a fair share of CPU time. It prevents any single request from blocking others. This improves responsiveness and user experience.]

### Example 2: [Mobile Applications]

**Description**: 
[Mobile apps often run background tasks such as downloading data while keeping the interface responsive.]

**Why Round-Robin works well here**: 
[Round-Robin allows background tasks and user interface tasks to share CPU time fairly. This keeps the app responsive and prevents freezing. It ensures smooth performance for the user.]

---

## Summary

**Key concepts I understood through these questions:**
1. 
2. 
3. 

**Concepts I need to study more:**
1. 
2. 
