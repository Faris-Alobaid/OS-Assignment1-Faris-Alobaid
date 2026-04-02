# Development Log

## Your Development Log:

### Entry 1 - [March 30, 2026, 6:00 PM]
**What I did**: Started understanding the assignment and running the base code

**Details**: 
- Read the assignment instructions carefully
- Reviewed Round Robin scheduling concept from the textbook
- Ran the original code to observe the output
- Identified how processes and threads are created and scheduled

**Challenges**: The output was complex at first and hard to follow

**Solution**: Carefully traced execution step-by-step and matched it with the code

**Time spent**: 1 hour

---

### Entry 2 - [March 31, 2026, 4:30 PM]
**What I did**: Implemented Feature 1 (Process Priority)

**Details**: 
- Added a priority variable inside the Process class
- Assigned random priority values to each process
- Created a getter method for priority
- Printed priority in the ready queue output

**Challenges**: Deciding where to initialize the priority value

**Solution**: Added it inside the constructor so every process gets a priority when created

**Time spent**: 1.5 hours

---

### Entry 3 - [April 1, 2026, 5:00 PM]
**What I did**: Implemented Feature 2 (Context Switch Counter)

**Details**: 
- Created a static counter variable in the main class
- Incremented the counter each time a new process is selected
- Printed total context switches at the end of the simulation

**Challenges**: Understanding where exactly context switching happens in the loop

**Solution**: Placed the counter increment right after polling from the queue

**Time spent**: 1 hour

---

### Entry 4 - [April 2, 2026, 3:00 PM]
**What I did**: Implemented Feature 3 (Waiting Time Tracking)

**Details**: 
- Added creationTime and waitingTime variables
- Used System.currentTimeMillis() to track time
- Calculated waiting time after each execution
- Displayed waiting time in the final summary

**Challenges**: Waiting time calculation was confusing at first

**Solution**: Used creation time as reference and updated waiting time after execution

**Time spent**: 2 hours

---

### Entry 5 - [April 2, 2026, 8:00 PM]
**What I did**: Testing, debugging, and finalizing the program

**Details**: 
- Ran the program multiple times to verify all features
- Checked correctness of priority, context switch count, and waiting time
- Cleaned up output formatting
- Prepared answers and documentation files

**Challenges**: Ensuring all features work together without conflicts

**Solution**: Tested each feature individually then combined them

**Time spent**: 1.5 hours

---

## Summary

**Total time spent on assignment**: ~7 hours

**Most challenging part**: Understanding how to correctly calculate waiting time and track execution flow

**Most interesting learning**: Learning how Round Robin scheduling works in real systems and how threads simulate CPU processes

**What I would do differently next time**: Start earlier and design features before coding to reduce debugging time
