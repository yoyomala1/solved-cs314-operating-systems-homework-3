Download Link: https://assignmentchef.com/product/solved-cs314-operating-systems-homework-3
<br>
5/5 - (1 vote)

Assignment- contact <a href="/cdn-cgi/l/email-protection#b5d4dbdedcc1d6dad1dcdbd2f5d2d8d4dcd99bd6dad8"><span class="__cf_email__" data-cfemail="82e3ece9ebf6e1ede6ebece5c2e5efe3ebeeace1edef">[email protected]</span></a> for other CS314 Assignments

1. (40 points) Implement semaphores using the pthread library. Consult the thread implementation in DLXOS for inspiration (semaphores are implemented in synch.h and synch.c).

Use pthread_mutex_lock and pthread_mutex_unlock (see man pthread mutex lock) to make the semaphore wait and post operations atomic.

Use pthread_cond_wait (see man pthread cond timedwait, but don’t use pthread cond timedwait) and pthread_cond_signal (see man pthread cond signal).Test your solution by implementing a simple rendezvous, e.g.:

THREAD A: THREAD B:printf(‘‘a1
’’); printf(‘‘b1
’’);sem_signal(aArrived); sem_signal(bArrived);sem_wait(bArrived); sem_wait(aArrived);printf(‘‘a2
’’); printf(‘‘b2
’’);

Your program should consistently print a1 and b1 before printing a2 and b2.

2. (10 points) Five jobs (A, B, C, D, and E), arrive in alphabetical order, and at almost the same time. They have estimated running times of 4, 5, 5, 3, and 8 minutes. Their priorities are 5, 4, 3, 2, and 1, respectively, with 5 being the lowest priority. The processes arrive in the following quanta: 1, 3, 3, 6, 10, respectively. For each of the following scheduling algorithms, determine the mean process turnaround time. Ignore process switching overhead and assume a quantum of 1 minute. Show your work for partial credit.• Round robin.• Priority scheduling.• First-come, first-served• Shortest-job first.

3. (10 pts) The aging algorithm with a = 1/2 is being used to predict run times. The previous four runs, from oldest to most recent, are 8, 12, 10, and 14 msec. What is the sequence of predicted runtimes starting with the first of the observed runs (8), ending with the predicted runtime after the last observed run (14). (See Tanenbaum’s section on Scheduling in RealTime Systems, Ch. 2)

4. (10 pts) A real-time system needs to handle one voice call that runs every 10 msec and consumes 4 msec of CPU time per burst, plus a video at 32 frames/sec, with each frame requiring 20 msec of CPU time. Is this system schedulable? Explain.

5. (10 pts) Consider a swapping system in which memory consists of the following hole sizes in memory order: 2KB, 8KB, 8KB, 6KB, 20KB, 8KB, 24KB, and 32KB. Which hole is taken for successive segment requests of 4KB, 8KB, and 16KB when each of the following algorithms is used:• First fit.• Best fit.• Next fit.• Worst fit.

6. (10 pts) For each of the following decimal virtual addresses, compute the virtual page number and offset for a 4KB page and for an 8KB page: 4097, 8193, 55555, 999999.