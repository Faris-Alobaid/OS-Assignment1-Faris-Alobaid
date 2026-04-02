# Reflection Questions

## Question 1: What did you learn about multithreading?

**Your Answer:**

Through this assignment, I learned how multithreading allows multiple tasks (threads) to run concurrently within the same process. I understood how to create threads in Java using the Runnable interface and how each process in the simulation is executed as a separate thread. I also learned about different thread states such as New, Runnable, Running, Waiting, and Terminated, and how threads move between these states during execution. One important concept I learned is that threads share the same memory space, which makes them more efficient than processes but also requires careful management. I also understood how the CPU scheduler (Round Robin in this case) controls which thread runs at a given time. What surprised me most is how context switching happens frequently and how it affects performance. Overall, this assignment helped me connect theoretical concepts from the operating systems course to practical implementation.

---

## Question 2: What was the most challenging part of this assignment?

**Your Answer:**

The most challenging part of this assignment was understanding how the scheduling loop works and how processes are re-added to the ready queue. At first, it was confusing to track how each thread executes for a time quantum and then gets paused and re-queued if not finished. Another difficult part was implementing the waiting time feature, because calculating time correctly using System.currentTimeMillis() required careful thinking. I also found it challenging to decide where exactly to place new features inside the existing code without breaking the logic. Understanding context switching and identifying the correct location to increment the counter was also tricky. These challenges were directly related to core operating system concepts like scheduling, process management, and CPU allocation.

---

## Question 3: How did you overcome the challenges you faced?

**Your Answer:**

I overcame these challenges by breaking the problem into smaller parts and focusing on one feature at a time. First, I carefully read the code and traced its execution step-by-step to understand how the scheduler works. I also referred to the textbook concepts from Operating System Concepts to better understand Round Robin scheduling and thread behavior. When implementing features, I tested each one separately before combining them, which helped me avoid bugs. For the waiting time calculation, I experimented with different approaches until I found a correct way using creation time. I also used debugging techniques such as printing intermediate values to verify correctness. This systematic approach helped me gradually build confidence and complete the assignment successfully.

---

## Question 4: How can you apply multithreading concepts in real-world applications?

**Your Answer:**

Multithreading is widely used in real-world applications to improve performance and responsiveness. For example, web browsers like Chrome use multiple threads to load web pages, play videos, and handle user input at the same time without freezing. Another example is mobile applications, where background threads handle tasks such as downloading data while the main thread keeps the user interface responsive. In gaming, threads are used to handle rendering, physics calculations, and user input simultaneously. In this assignment, the Round Robin scheduler ensures fairness among processes, which is similar to how operating systems manage multiple applications running on a computer. Multithreading allows better CPU utilization and faster execution of tasks. Overall, these concepts are essential in building efficient and responsive software systems.

---

## Additional Reflections (Optional)

### What would you like to learn more about?

I would like to learn more about advanced scheduling algorithms such as Priority Scheduling and Multilevel Queue Scheduling. I am also interested in learning about synchronization techniques like mutexes and semaphores to manage shared resources safely. Additionally, I would like to explore how deadlocks occur and how operating systems prevent them. Understanding real-world implementations of thread management in modern operating systems would also be valuable.

---

### How confident do you feel about multithreading concepts now?

**Rating:** Intermediate

I feel that I have a good understanding of the basic concepts such as thread creation, scheduling, and execution. I can now explain how Round Robin works and how threads interact within a program. However, I still need more practice with advanced topics like synchronization, race conditions, and deadlocks. With more hands-on experience, I believe I can reach a higher level of confidence.

---

### Feedback on the assignment

This assignment was very helpful in understanding operating system concepts in a practical way. It allowed me to connect theory with real implementation, especially in scheduling and multithreading. The difficulty level was moderate, as it required both coding skills and conceptual understanding. However, some parts could be clearer, especially instructions for implementing additional features. Overall, it was a valuable learning experience and improved my understanding of CPU scheduling.
