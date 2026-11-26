<img width="1917" height="1098" alt="image" src="https://github.com/user-attachments/assets/48320cba-c7f0-413e-ba02-47e961320956" /># 📝 MY_WORK: Student Information, Development Log, Reflection & Answers

> This is the **only file** your instructor reads to grade Parts 3 and 4 (documentation and video). Everything you write here must be **in your own words**.

---

## 🛑 STOP: Read This Before You Do Anything Else

> ### 1️⃣ Read the whole `README.md` first
> The `README.md` in this repository contains the full instructions: how this assignment continues Assignment 1, the Chapter 5 recap, class descriptions, feature specifications, question prompts and the video script. **If you skip it, you will lose marks.**
>
> ### 2️⃣ Understand the full code before answering any question
> Open `SchedulerSimulationSync.java` and read it **from top to bottom**. You must be able to explain what `SharedStats`, `ReadyQueue`, `CpuWorker`, `RaceWindow.pause()`, `ReentrantLock` and `Semaphore` do **before** you write a single answer in Parts B and C. **Run the original starter first** (it is intentionally broken) and **save its output**: you need it for Question 1 of Part C.
>
> ### 3️⃣ Use only the code of this repository
> Work **only** on `SchedulerSimulationSync.java` from this repository. Do **not** copy or paste code from your previous assignments.
>
> ### 4️⃣ Commit many times, not once
> A single commit, or all commits made in the last hour, costs you **-0.5 mark**. See the [Commit Rules](#-commit-rules-mandatory) below.

**How to use this file:**
1. Fill in your **Student Information** (below) right now.
2. Follow the steps in the **Work Roadmap** in order.
3. Update the **Development Log** *every time* you work on the assignment, not at the end.
4. Do not delete any section header. Replace the `[...]` placeholders with your own text.

---

## 👤 Student Information

> ⚠️ **WARNING:** Fill this in first. Your name and ID must match the student ID you set in `SchedulerSimulationSync.java` (line 304) and the one you say in your video.

| Field | Your Answer |
|-------|-------------|
| **Full Name** | [سعد عبدالعزيز الهليل] |
| **Student ID** | [446050203] |
| **University Email** | 446050203@std.psau.edu.sa |
| **GitHub Username** | saad-abdulaziz-2222  |
| **Repository Link** | https://github.com/saad-abdulaziz-2222/OS-Assignment3--Saad-Hilayel |
 
---

## 🎥 Video Link

**Video Link**:[ https://drive.google.com/file/d/1UhV_TV5l5_ozLsuSM_cR98QS9WlSvGOj/view](https://drive.google.com/file/d/1UhV_TV5l5_ozLsuSM_cR98QS9WlSvGOj/view?usp=sharing)

> ⚠️ **WARNING:** The video must be **publicly accessible** ("Anyone with the link can view") on **Google Drive**, **YouTube (Unlisted or Public)** or any other cloud file-sharing system. A private, restricted or broken link counts as a **missing video (-1 mark)**.
>
> 💡 **TIP:** Open the link in a **private/incognito window** before you submit. If it asks you to log in or request access, it is not public.
>
> 📌 **NOTE:** The link goes in **this file only** (`MY_WORK.md`), **not** in `README.md`. Name your video file `StudentID_Assignment3_Demo.mp4`. It must last **2 to 3 minutes**.

---

## 🗺️ Work Roadmap (follow in this order)

| Step | What to do | Where | Marks |
|:----:|------------|-------|:-----:|
| 0 | Read `README.md`, read the full code, **run the original starter and save its output** (it fails on purpose) | Your IDE | – |
| 1 | Fork, rename, keep the repo **PUBLIC**, set your student ID (line 304), **commit** | GitHub + code | Part 1 (1) |
| 2 | Feature 1: Mutex lock on the ready queue, **commit** | Code | Part 2 (0.25) |
| 3 | Feature 2: Mutex lock(s) on the shared statistics, **commit** | Code | Part 2 (0.25) |
| 4 | Feature 3: Counting semaphore instead of busy waiting, **commit** | Code | Part 2 (0.5) |
| 5 | Development Log (5+ entries, different dates) | This file, Part A | Part 3 (0.5) |
| 6 | Reflection (4 questions) | This file, Part B | Part 3 (0.5) |
| 7 | Technical Answers (4 questions) | This file, Part C | Part 3 (0.5) |
| 8 | Record the video, upload it, paste the link above | Video + this file | Part 4 (1.5) |
| 9 | Final check, then submit the repo link on Blackboard | Blackboard | – |

> 💡 **TIP:** Tick each step off as you go. Do not leave the log, the reflection or the video for the last day.

---

## 🔁 Commit Rules (MANDATORY)

> ### ⚠️ MANY COMMITS ARE REQUIRED. A single bulk commit is penalized (-0.5 mark).

**Minimum: 4 meaningful commits. Aim for 7 or more.**

| # | Commit | Example message |
|:-:|--------|-----------------|
| 1 | Student ID set | `Set my student ID: 441234567` |
| 2 | Feature 1: Ready queue lock | `Feature 1: Protected the ready queue with a ReentrantLock` |
| 3 | Feature 2: Statistics locks | `Feature 2: Added locks to the shared statistics counters` |
| 4 | Feature 3: Semaphore | `Feature 3: Replaced busy waiting with a counting semaphore` |
| 5 | Development log entries | `Docs: Added development log entries 1-3` |
| 6 | Reflection and answers | `Docs: Completed reflection and technical answers` |
| 7 | Video link | `Docs: Added demo video link` |

**Rules:**
- ✅ **One commit per feature.** Do not put all three features in one commit.
- ✅ **Commit after each work session**, and after each part of this file.
- ✅ **Spread your commits over different dates.** Not all in one day.
- ❌ **Do not make all commits in the last hour** before the deadline (November 14, 2026).
- ❌ **No vague messages** like `done`, `update` or `final version`.

> 💡 **TIP:** Your commit history is checked and you **show it in your video** (at least 4 commits visible). Your development log dates should match your commit dates.
>
> 💡 **TIP:** **Use VS Code** (see *Recommended Development Environment* in `README.md` for the full setup). Sign in to GitHub in VS Code, then commit from the Source Control panel (Ctrl+Shift+G) → stage → write a message → Commit → Sync/Push. You can edit and commit this file the same way. **Pushing** matters: commits that are not pushed to GitHub are invisible to the instructor.

---

# Part A: Development Log (0.5 mark)

> ⚠️ **WARNING:** Minimum **5 entries**, spread over **different dates**. Five entries written on the same day, or written all at once at the end, will lose marks and look like a copy. Entry dates should be **between the start of the assignment and the deadline (November 14, 2026)**.
>
> 💡 **TIP:** Write an entry at the **end of each work session**, while you still remember what happened. It takes 5 minutes.
>
> 💡 **TIP:** Be specific. "Worked on the code" is a weak entry. "Added a `ReentrantLock queueLock` to `ReadyQueue` and wrapped the body of `poll()` in `lock()` / `try` / `finally { unlock() }`" is a strong one.
>
> 📌 **NOTE:** Each entry needs: date and time, what you did, details, challenges, solution, and time spent. Real challenges are fine (and expected). Do not invent fake ones.

## Example Entry (do not copy it, write your own)

### What I did: Set my student ID and tested the original starter code.

### Entry 1 - [November 25, 2026, 6:33 AM]

What I did: Set my student ID and tested the original starter code.

Details:

Set my actual student ID (446050203) in SchedulerSimulationSync.java.

Ran the original starter code before implementing the synchronization features.

Observed errors caused by concurrent access to the shared ready queue.

Saved the original output for comparison with the final version.

Challenges: The original program failed when multiple CPUs accessed the ready queue at the same time.

Solution: Examined the error messages and the shared queue operations to understand where synchronization was needed.

 Time spent: [40 minutes]
---

### Entry 2 - [November 25, 2026, 7:44 AM]

What I did: Implemented Feature 1: Ready Queue Lock.

Details:

Imported ReentrantLock.

Added queueLock inside the ReadyQueue class.

Protected add(), poll(), processOf(), and snapshot() using lock(), try, and finally.

Ensured that only one CPU could access the shared queue at a time.

Challenges: Making sure all shared queue operations were protected without changing the original scheduling logic.

Solution: Used the same lock for all operations involving the shared list and map, and released it inside a finally block.

Time spent: [1:15 hour]

---

### Entry 3 - [November 25, 2026, 9:43 AM]

What I did: Implemented Feature 2: Statistics Locks.

Details:

Added a ReentrantLock named statsLock inside SharedStats.

Protected incrementContextSwitch(), incrementCompletedProcess(), and addServiceTime().

Also protected the three getter methods.

Used one lock to protect all three shared statistics.

Challenges: Understanding why reading and updating shared counters could cause lost updates when multiple threads executed simultaneously.

Solution: Used one lock for all three statistics and applied try/finally to ensure the lock was always released.

Time spent: [2 hours]
---

### Entry 4 - [November 25, 2026, 4:13 PM]

What I did: Fixed a brace and code-placement issue.

Details:

Reviewed the class structure after adding the synchronization methods.

Found an issue with the placement of closing braces.

Corrected the structure to ensure the methods belonged to the correct class.

Checked that the code structure was valid before continuing.

Challenges: Some methods were not placed inside the correct class because of an extra or misplaced closing brace.

Solution: Reviewed the class boundaries and corrected the braces and method placement.

Time spent: [5 minutes]

---


### Entry 5 - [November 25, 2026, 5:25 PM]

What I did: Implemented Feature 3: Counting Semaphore.

Details:

Imported Semaphore and initialized readyCount to zero.

Added readyCount.release() when a process is added to the ready queue.

Added waitForProcess() using readyCount.acquire().

Replaced the busy-waiting section in CpuWorker with blocking semaphore waiting.

Added shutdown logic to wake up CPUs when all processes have completed.

Ran the final simulation and checked the verification results.

Challenges: Understanding how to wake up CPUs that were blocked on the semaphore after all processes had finished.

Solution: Added wakeUpAllCPUs() to release enough permits for the CPU threads to wake up and terminate.

Time spent: [2:30 hours]
---

## Development Log Summary

> 💡 **TIP:** Fill this in **last**, after all entries are written.

Total time spent on assignment: [6:30 hours]

Most challenging part: Implementing the counting semaphore and making sure all CPU threads terminated correctly after the final process completed.

Most interesting learning: Understanding how synchronization prevents race conditions and how a semaphore allows threads to block instead of continuously checking an empty queue.

What I would do differently next time: I would study the synchronization concepts and plan the implementation more carefully before making changes to the code.

---

# Part B: Reflection (0.5 mark)

> 🛑 **STOP:** Do **not** start this part until you have read the `README.md`, read the **entire** `SchedulerSimulationSync.java`, run it, and finished the three features.
>
> ⚠️ **WARNING:** Each answer must be **5 to 7 sentences**, in **your own words**. Copied or AI-generated answers without understanding get **0 marks for the whole assignment**. You may be asked to explain them in person.
>
> 💡 **TIP:** Mention concrete things you actually did: a method you wrote, an error you hit, a line of output you saw. Generic answers score low.
>
> 💡 **TIP:** Draft your answer in a few bullet points first, then turn them into sentences.

## Question 1: What did you learn about synchronization?

> 💡 **TIP:** Talk about race conditions (read-modify-write), critical sections, mutual exclusion with `ReentrantLock` and `try/finally`, the role of a counting semaphore, and what surprised you when the starter failed.

**Your Answer:** *(5-7 sentences)*

[It is clear that synchronization helps resolve any issues arising from having multiple CPUs trying to access shared data. Lost updates may occur in case of race condition where threads modify the same variable. I utilized ReentrantLock to synchronize access to the ready queue and shared statistics. Another thing that I learned is that the use of counting semaphore causes CPUs to wait until a process appears.
.]

## Question 2: What was the most challenging part of this assignment?

> 💡 **TIP:** Pick **one** specific challenge (understanding why the starter failed, choosing the lock granularity, the initial value of the semaphore, the shutdown of the CPUs, Git, the video) and say *why* it was hard.

**Your Answer:** *(5-7 sentences)*

[The toughest part was the implementation of feature number 3 and the shutdown of the CPUs. I knew how to use the release() and acquire() methods, but getting all the CPUs to shut down properly was a problem. This is because some CPUs might get stuck even when all the processes are done. To address that, I implemented the wakeUpAllCPUs() method.
]

## Question 3: How did you overcome the challenges you faced?

> 💡 **TIP:** Describe your method: reading the slides and the documentation, adding `System.out.println` to debug, running the program many times, re-reading the README, testing after each small change, asking for help.

**Your Answer:** *(5-7 sentences)*

[I have done the assignment by working on one feature at a time. First, I ran the program and analyzed the errors in it. After that, I added locks to the ready queue and to shared statistics. After that, I added semaphores and shutdown functionality to it. Lastly, I ran the test again and verified the result.
]

## Question 4: Where can synchronization concepts be applied in real-world applications?

> 💡 **TIP:** Use real applications you know (banking and money transfers, ticket or seat booking, a shared counter on a website, a print queue, a database) and connect each one to what you built here (shared data, critical section, lock or semaphore).

**Your Answer:** *(5-7 sentences)*

[Synchronization plays a key role in areas where several users need to access common resources. Synchronization is used in banks to avoid improper account balance adjustment, synchronization is required in the process of booking seats for two customers in the ticket booking system. Printing queues use synchronization for print jobs by using semaphores.]

### Optional: What would you like to learn more about?

[Any topics related to synchronization or operating systems that you're curious about?]

### Optional: How confident do you feel about synchronization concepts now?

[Beginner / Intermediate / Confident. What do you understand well? What needs more practice?]

### Optional: Feedback on the assignment

[Any comments? Was it helpful? Too easy or hard? Suggestions?]

---

# Part C: Technical Answers (0.5 mark)

> 🛑 **STOP:** You cannot answer these questions without understanding the code. Re-read `SchedulerSimulationSync.java` and **run it** first. Your answers must reference **your own code and your own output** (your student ID makes your output and your expected values unique).
>
> ⚠️ **WARNING:** Each answer must be **3 to 5 sentences**, with specific examples from your code or output. Use correct terms: race condition, critical section, mutual exclusion, mutex lock, semaphore, busy waiting, deadlock, producer, consumer.
>
> 💡 **TIP:** Keep the output of the **original starter** and the output of your **final version** in text files or screenshots, so you can copy real snippets for Question 1.

## Question 1: Race Condition in Your Own Output

**Question**: Run the **original starter** (before any fix) and paste the **verification block** of that run. Which value was wrong (expected vs observed)? Explain **step by step**, with two named threads/CPUs, how **one lost update** happens on one of the shared variables (read, `RaceWindow.pause()`, write). Why can the same bug happen on a real machine even without `RaceWindow`, and why is it hard to detect?

> ⚠️ **WARNING:** The snippet must come from **your own run** (with your student ID), not from a classmate or from this README.
>
> 💡 **TIP:** Use a small timeline: *CPU-1 reads `contextSwitchCount` = 12 → CPU-2 reads 12 → CPU-1 writes 13 → CPU-2 writes 13 → one increment is lost.* If your starter run crashed before printing numbers, run it several times (or paste the exception and the watchdog message and explain it).

**Your Answer:** *(3-5 sentences)*

[In the first execution, the four threads of CPU faced the problem of NullPointerException in ReadyQueue.snapshot() due to access by more than one CPU to the common queue without any synchronization. Verification had produced the expected results of 32 context switches, 17 processes finished, and 94831 ms service time, yet all three had their observed values equal to zero. Lost update may occur when CPU-1 reads the contextSwitchCount = 12 and CPU-2 reads the same value in RaceWindow.pause() and then both write the value 13 resulting in losing an increment. It may occur on the actual machine as well without RaceWindow.]

Verification block of the **original starter**:
```
Exception in thread "CPU-3"
java.lang.NullPointerException: Cannot read field "next" because "this.next" is null
    at java.base/java.util.LinkedList$ListItr.next(Unknown Source)
    at ReadyQueue.snapshot(SchedulerSimulationSync.java:168)
    at CpuWorker.run(SchedulerSimulationSync.java:320)

Context switches (quanta executed) expected 32 observed 0 MISMATCH
Completed processes expected 17 observed 0 MISMATCH
Total service time (ms) expected 94831 observed 0 MISMATCH
Busy-waiting polls (must be 0) expected 0 observed 0
```

Verification block of **my final version**:
```
Context switches (quanta executed) expected 32 observed 32
Completed processes expected 17 observed 17
Total service time (ms) expected 94831 observed 94831
Busy-waiting polls (must be 0) expected 0 observed 0

All shared values are consistent.
```

**Explanation of the timeline:**
CPU-1 reads the counter as 12. CPU-2 also reads 12 before CPU-1 writes its result. CPU-1 writes 13, then CPU-2 writes 13. The final value is 13 instead of 14, so one update is lost.

## Question 2: Critical Sections and Lock Granularity

**Question**: List the **critical sections** you protected (variables and methods) and the lock(s) you used. **Lock granularity:** did you use **one lock** for the three statistics or **one lock per variable**? Why, and what is the trade-off? Why is the **ready queue** protected by a **different** lock than the statistics? Explain how your solution provides **mutual exclusion**, and discuss **progress** and **bounded waiting** (a default `ReentrantLock` is not fair: what does that imply?).

> 💡 **TIP:** The three counters are independent: does updating `contextSwitchCount` need to block an update of `totalServiceTime`? Also think about what could go wrong (deadlock, or long waiting) if the queue lock and the statistics lock were the **same** lock and a thread held it while doing something slow.

**Your Answer:** *(3-5 sentences)*

[QueueLock was used to synchronize readyQueue and the list and map that belong to it. I have created only one statsLock for the three statistics and corresponding getter methods since it simplifies synchronization even though it makes it impossible to update the statistics independently. ReadyQueue has its own lock since it protects other shared data. Using lock() method with finally and unlock() method allows mutual exclusion and releasing of the lock. But default ReentrantLock is not fair so a thread can wait longer than others and bounded waiting is not ensured.]

| Critical section (variable / method) | Lock used | Why it needs protection |
|ReadyQueue.add()| queueLock | Protects adding threads to the list and map. |
|ReadyQueue.poll()| queueLock | Prevents multiple CPUs from removing the same queue item. |
|ReadyQueue.processOf()| queueLock |Protects access to the process map. |
|ReadyQueue.snapshot()| queueLock |Protects iteration over the shared queue. |
|SharedStats.incrementContextSwitch()| statsLock |Prevents lost counter updates. |
|SharedStats.incrementCompletedProcess()| statsLock |Prevents lost counter updates. |
|SharedStats.addServiceTime()| statsLock |Protects the shared service-time total. |
|SharedStats.getCompletedProcessCount()| statsLock |Protects reading the completed counter. |
|SharedStats.getContextSwitchCount()| statsLock |Protects reading the context-switch counter. |
|SharedStats.getTotalServiceTime()| statsLock |	Protects reading the service-time total. |
## Question 3: Busy Waiting vs Semaphore

**Question**: Describe the **busy waiting** of the starter and its cost (give the `Busy-waiting polls` number from your **starter** run). What does the **value of your semaphore** represent? What is its **initial value** and why? What is its value right after the `numProcesses` initial `add()` calls? Why does the last CPU call `release(totalCPUs)` at the end, and what would happen if it did not?

> 💡 **TIP:** Think about what a CPU does when the queue is empty in the starter, and what a CPU does in your final version (is it running, ready or blocked?). Also check what happens to a CPU blocked in `acquire()` when no process will ever be added again.

**Your Answer:** *(3-5 sentences)*

[In the first starter code, CPUs were constantly scanning the ready queue and sleeping for 20 milliseconds whenever the ready queue was empty, thereby wasting CPU cycles. In my final code, I made use of a counting semaphore called readyCount that is responsible for keeping count of the number of available processes in the queue. The starting value of the counting semaphore is 0 since no processes are initially available, and after adding the initial processes, the value of the semaphore becomes 17. The function release() increments the permits while acquire() decrements the permits and blocks the CPU.]

## Question 4: Classical Problems and Deadlock

**Question**: The CPUs and the ready queue look like a classical synchronization problem of Chapter 5. **Name it**, and say who plays the **producer** and the **consumer** roles (careful: here the CPUs also re-enqueue processes). If the ready queue were **bounded** (capacity `K`), name the **three semaphores** you would need and their **initial values**. Describe a **deadlock scenario** that appears if a thread acquired the **mutex before** waiting on the semaphore (or if two locks were acquired in different orders), and say **which of the four necessary conditions** you would break to prevent it.

> 💡 **TIP:** Recall the bounded-buffer solution of the slides (`empty`, `full`, `mutex`) and the order of `wait()` calls in the producer and the consumer. For the deadlock, think about a producer that holds the mutex while waiting for a free slot that only a consumer (who needs the mutex) can create.

**Your Answer:** *(3-5 sentences)*

**Classical problem and roles**:
[The ready queue implements the classical producer-consumer problem, where the primary thread is the producer and the CPUs are the consumers. The CPUs are also producers whenever they re-enqueue the process that is not finished yet.
]

**Semaphores for a bounded queue (name and initial value)**:
[In case of a bounded queue with capacity of K, there will be three semaphores: empty, which has K as the initial value, full, whose initial value is 0, and mutex, whose initial value is 1.
]

**Deadlock scenario and prevention**:
[A deadlock can arise if the producer takes the mutex lock when the buffer is full and waits for an empty place in the buffer. The consumer cannot dequeue the item and signal the empty semaphore since it requires the same mutex lock. To avoid this deadlock situation, the producer must take empty before taking mutex.
]

## Summary

**Key concepts I understood through these questions:**
How race conditions happen and how lost updates can occur when multiple threads access shared data.

How ReentrantLock provides mutual exclusion and protects critical sections.

How counting semaphores coordinate threads and prevent busy waiting

**Concepts I need to study more:**
Deadlock conditions and how to prevent them.

Different lock strategies, fairness, and bounded waiting.

---

# ✅ Final Checklist (complete before submitting)

> ⚠️ **WARNING:** Go through every line. Blackboard does not accept submissions after the deadline, which is **November 14, 2026**.

**Repository**
- [ ] Repository is **PUBLIC** (Settings → Danger Zone → Visibility)
- [ ] Repository is renamed to `OS-Assignment3-YourFirstName-YourLastName`
- [ ] GitHub account uses the university email (`@std.psau.edu.sa`)

**Code**
- [ ] Student ID is set in `SchedulerSimulationSync.java` (line 304)
- [ ] My code is based **only** on the starter of this repository (nothing copied from previous assignments)
- [ ] Code compiles and runs with no errors, and terminates by itself (no `⛔ WATCHDOG`)
- [ ] Feature 1 (ready queue lock), Feature 2 (statistics locks) and Feature 3 (semaphore, no busy waiting) all work
- [ ] **The four verification lines are ✔ in 5 consecutive runs**
- [ ] Every lock is released in a `finally` block
- [ ] `RaceWindow`, `Config`, the verification block and the watchdog are **unchanged**
- [ ] Each feature has clear comments

**Commits**
- [ ] **At least 4 meaningful commits, ideally 7 or more**
- [ ] **One commit per feature**
- [ ] Commits are spread over **different dates** (not all in the last hour)
- [ ] Everything is **pushed** to GitHub

**This file (`MY_WORK.md`)**
- [ ] Full name and student ID filled in at the top
- [ ] Development log has **5+ entries** on different dates
- [ ] Reflection: 4 questions, 5-7 sentences each
- [ ] Technical answers: 4 questions, 3-5 sentences each, with examples from **your** output (starter output **and** final output pasted in Question 1)
- [ ] No `[...]` placeholders left
- [ ] No section headers deleted

**Video**
- [ ] 2-3 minutes long, named `StudentID_Assignment3_Demo.mp4`
- [ ] Shows your name, ID, repository, 3 features (and your lock granularity choice), IDE execution with the verification block, one synchronization concept, and commit history
- [ ] Link is **public** (tested in an incognito window) and pasted in the **Video Link** section above

**Blackboard**
- [ ] Submit **only** the link to your public GitHub repository

> 🎯 **Good luck!** Start early, commit regularly, and make sure you can explain every line you submit.
