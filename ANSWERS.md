# Assignment Questions

## Instructions
Answer all 4 questions with detailed explanations. Each answer should be **3-5 sentences minimum** and demonstrate your understanding of the concepts.

---

## Question 1: Thread vs Process

**Question**: Explain the difference between a **thread** and a **process**. Why did we use threads in this assignment instead of creating separate processes?

**Your Answer:**

[A process is an independent program that has its own memory and resources, while a thread is a smaller unit of execution within the same process and shares the same memory. Processes are heavier and require more time to create and manage, while threads are lighter and faster. The main difference is that processes are completely separate, while threads run within the same environment. We used threads in this assignment because they are easier to manage, faster to execute, and more suitable for simulating a CPU scheduler.]

---

## Question 2: Ready Queue Behavior

**Question**: In Round-Robin scheduling, what happens when a process doesn't finish within its time quantum? Explain using an example from your program output.

**Your Answer:**

[In Round-Robin scheduling, if a process does not finish within its time quantum, it is removed from the CPU and placed back at the end of the ready queue. This means it will wait for its turn again after the other processes execute. In my program, this appears when a process prints that it "yields CPU for context switch" and then gets added back to the queue. For example, a process like P5 runs for its quantum, then is re-enqueued and runs again later until it finishes.
 ]

Example from my output:
```

P5 yields CPU for context switch  
P5 added to ready queue  
```

**Explanation of example:**

This shows that P5 did not finish execution within its time quantum, so it was moved to the back of the ready queue. It will wait until other processes run before getting CPU time again.

---

## Question 3: Thread States

**Question**: A thread can be in different states: **New**, **Runnable**, **Running**, **Waiting**, **Terminated**. Walk through these states for one process (P1) from your simulation.

**Your Answer:**

1. **New**: P1 is in the New state when it is first created using the Process constructor but before the thread starts.

2. **Runnable**: P1 becomes Runnable after the thread is created and added to the ready queue, waiting for CPU scheduling.

3. **Running**: P1 is in the Running state when the scheduler selects it and the thread starts executing using start().

4. **Waiting**: P1 enters the Waiting state when it calls sleep() during execution, pausing temporarily before continuing.

5. **Terminated**: P1 reaches the Terminated state when it finishes execution and its remaining time becomes zero.
---

## Question 4: Real-World Applications

### Example 1: Web Servers
Web servers handle multiple user requests at the same time using threads. Round-Robin scheduling helps distribute CPU time fairly between requests so no user has to wait too long. This improves responsiveness and performance when many users access the server simultaneously.

### Example 2: Operating Systems
Operating systems use Round-Robin scheduling to manage processes and threads efficiently. Each process gets a fixed time quantum, ensuring fairness and preventing any single process from taking all CPU time. This makes the system stable and responsive for all running applications.

## Summary

**Key concepts I understood through these questions:**
1. The difference between threads and processes and how they manage resources.
2. How Round-Robin scheduling works and how processes are re-added to the ready queue.
3. The different thread states and how a process moves through them during execution.

**Concepts I need to study more:**
1. Advanced multithreading concepts like synchronization and avoiding race conditions.
2. How operating systems handle large numbers of threads efficiently in real-world systems.