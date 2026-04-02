# Assignment Questions

## Instructions
Answer all 4 questions with detailed explanations. Each answer should be **3-5 sentences minimum** and demonstrate your understanding of the concepts.

---

## Question 1: Thread vs Process

**Question**: Explain the difference between a **thread** and a **process**. Why did we use threads in this assignment instead of creating separate processes?

**Your Answer:**

[A process is an independent program that is running and has its own memory space, resources, and system state. A thread, on the other hand, is a small unit of execution that lives inside a process and shares memory and resources with other threads in that process. Making processes is more expensive because it means giving them their own memory and system resources. Threads, on the other hand, are faster and easier to make and manage.]

---

## Question 2: Ready Queue Behavior

**Question**: In Round-Robin scheduling, what happens when a process doesn't finish within its time quantum? Explain using an example from your program output.

**Your Answer:**

[If a process doesn't finish within its time quantum in Round-Robin scheduling, it is stopped and put at the end of the ready queue. This makes sure that all processes have an equal chance to run and stops one process from taking over the CPU. The process will stay in line until it gets its turn again.]

Example from my output:
```
[Paste a relevant snippet from your program output here showing a process being re-queued]
```

**Explanation of example:**
[Explain what's happening in the output snippet you pasted]

---

## Question 3: Thread States

**Question**: A thread can be in different states: **New**, **Runnable**, **Running**, **Waiting**, **Terminated**. Walk through these states for one process (P1) from your simulation.

**Your Answer:**

[New:
When the thread object is made with new Thread(process), but before the start() method is called, P1 is in the New state.
Runnable:
After calling start(), P1 goes into the Runnable state. At this point, it is ready to run and is waiting for the CPU scheduler to give it some CPU time.
Running:
When the CPU runs the run() method on P1, it is in the Running state. This is where it does its quantum execution and updates its remaining time.
Waiting:
Thread can put P1 in the Waiting state.Inside the run method, sleep() is called to make it look like the program is running. The thread is not doing anything during this time.
End:
When P1 is done running, it goes to the Terminated state, which means its remaining time is zero and the thread is done running.]

1. **New**: [When is P1 in New state?]

2. **Runnable**: [When does P1 become Runnable?]

3. **Running**: [When is P1 Running?]

4. **Waiting**: [When/why would P1 be Waiting?]

5. **Terminated**: [When is P1 Terminated?]

---

## Question 4: Real-World Applications

**Question**: Give **TWO** real-world examples where Round-Robin scheduling with threads would be useful. Explain why this scheduling algorithm works well for those scenarios.

**Your Answer:**

### Example 1: [A web server that can handle many requests]

**Description**: 
[What it is:
A web server can handle many client requests at once, with each request being handled in its own thread.

Why Round-Robin works well in this case:
Round-Robin makes sure that all client requests get a fair amount of CPU time without starving. It makes the system more responsive by letting each request be handled in small time slices, which stops long requests from blocking others.]

**Why Round-Robin works well here**: 
[Explain why Round-Robin scheduling is suitable. Consider fairness, responsiveness, predictability, etc.]

### Example 2: [Time-Sharing Operating Systems]

**Description**: 
[What it is:
In time-sharing systems, several users can use the same computer at the same time through terminals, each running a different program.

Why Round-Robin works well in this case:
Round-Robin scheduling is fair because it gives all users the same amount of CPU time. It makes sure that response times are fast and that no one user can take over system resources, which is important for interactive systems.]

**Why Round-Robin works well here**: 
[What it is:
With time-sharing systems, multiple people can use the same computer at the same time through terminals, each running a different program.

Why Round-Robin is a good choice here:
Everyone gets the same amount of CPU time with round-robin scheduling, which is fair. It makes sure that response times are quick and that no one user can take over system resources, which is important for systems that people use.]

---

## Summary

**Key concepts I understood through these questions:**
1. What makes threads better than processes in simulations and how they are not the same
2. How Round-Robin scheduling makes sure everyone gets a fair chance with a circular ready queue
3. The life cycle of a thread and how it moves from one state to another

**Concepts I need to study more:**
1. Accurate calculation of waiting time vs turnaround time
2. Advanced scheduling algorithms like Multilevel Queue and Priority Scheduling
