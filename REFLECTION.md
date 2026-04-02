# Reflection Questions

## Instructions
Answer the following questions about your learning experience. Each answer should be **at least 5-7 sentences** and show your understanding.

---

## Question 1: What did you learn about multithreading?

**Your Answer:**

[From this assignment, I learned that multithreading allows a program to handle more than one task in a controlled way. I understood that each process in this simulation can be represented as a thread, and the scheduler decides when each thread gets CPU time. I also learned how methods like `start()`, `join()`, and `sleep()` are used to manage the execution of threads. One important thing I noticed is that threads may run independently, but they still need coordination so the program behaves correctly. This assignment also helped me understand how time quantum affects fairness between processes in Round Robin scheduling. Overall, I learned that multithreading is not only about running tasks at the same time, but also about organizing and controlling execution carefully.]

---

## Question 2: What was the most challenging part of this assignment?

**Your Answer:**

[The most challenging part of this assignment was implementing the new features without breaking the original scheduling logic. In particular, I found the waiting time calculation difficult because the process can enter the ready queue multiple times before it finishes. It was not always easy to know the exact moment when waiting starts and when it should be updated. Another challenge was dealing with code errors caused by small mistakes such as wrong variable names or misplaced braces. I also had to be careful when modifying the constructor and process creation after adding the priority field. This made the assignment challenging because it required both understanding the code structure and checking many details carefully.]

---

## Question 3: How did you overcome the challenges you faced?

**Your Answer:**

[I overcame the challenges by working on the assignment step by step instead of trying to finish everything at once. I focused on one feature at a time, tested it, and then moved to the next part after making sure the previous change was working. When I faced errors, I reviewed the code carefully and compared it with the assignment requirements until I found the issue. I also used debugging in a simple way by reading the output and checking which part of the program was not behaving correctly. Breaking the problem into smaller parts helped me stay organized and reduced confusion. In the end, this approach made the assignment easier to complete and helped me understand the code better.]

---

## Question 4: How can you apply multithreading concepts in real-world applications?

**Your Answer:**

[Multithreading is used in many real-world applications to handle multiple tasks efficiently at the same time. For example, web browsers use threads to load different tabs and process user input without freezing the interface. In mobile apps, one thread can handle the user interface while another performs background tasks like loading data from the internet. Games also use multithreading to manage graphics, sound, and user actions simultaneously. Operating systems use scheduling algorithms like Round Robin to distribute CPU time fairly between processes, similar to what we implemented in this assignment. This shows how multithreading helps improve performance and responsiveness in real systems.]

---

## Additional Reflections (Optional)

### What would you like to learn more about?

[I would like to learn more about advanced concepts in multithreading such as synchronization and avoiding race conditions. I am interested in understanding how threads safely share data without causing errors. I also want to explore how operating systems manage large numbers of threads efficiently. Learning about deadlocks and how to prevent them is something I find important. In addition, I would like to understand how multithreading is optimized in real-world systems. This would help me build stronger and more reliable programs in the future.]

---

### How confident do you feel about multithreading concepts now?

[I would describe my level as intermediate because I now understand the basic concepts of multithreading and scheduling. I feel comfortable working with threads, creating them, and controlling their execution using methods like start and join. I also understand how time quantum affects process execution in scheduling algorithms. However, I still need more practice with advanced topics like synchronization and handling shared resources. Sometimes I need extra time to fully understand complex behaviors in multithreading. With more practice, I believe I can improve my confidence further.]



---

### Feedback on the assignment

[This assignment was very useful in helping me understand how CPU scheduling and multithreading work in practice. It allowed me to connect theoretical concepts with actual implementation in code. The assignment was a bit challenging, especially when adding new features without breaking the existing logic. However, the challenge helped me improve my problem-solving and debugging skills. I think the assignment could be improved by providing slightly more guidance for complex features. Overall, it was a valuable experience that helped me learn important concepts in operating systems.]
