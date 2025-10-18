## Process
A process is a running program. When application program are used, processes are being created and ran. A process can be thought of as an entity that consists of two main elements, program code and a set of data. When a program is being executed by the CPU, a process is created. 

## Process States
A program can be divided into two types:
- Running
- Not Running

<p align="center">
<img width="719" height="232" alt="image" src="https://github.com/user-attachments/assets/00ae31fb-d47f-4273-8bbe-7f72da32cf04" /> <br>
Figure 5.1 Two state process model
</p>

In a realistic world, there are more than 2 types of processes:
1. New Process
2. Ready Process
3. Running Process
4. Blocked / Waiting Process
5. Terminated Process
6. Zombie Process
7. Orphan Process
8. Daemon Process

However, for academic degree purpose, we will only touch on 5 of the processes.
1. New Processes (Processes has been created but has not been admitted into the ready queue for CPU scheduling)
3. Ready Processes (Process has been given the resources and waiting for CPU time to execute)
4. Running Processes (Process that is currently being executed by the CPU)
5. Blocked Processes (Process that has been temporarily halted until the resource it requires becomes available)
6. Exit (Process has finish execution)

<p align="center">
<img width="1177" height="493" alt="image" src="https://github.com/user-attachments/assets/30d53c08-ff56-4114-a41f-17190ae867a4" /><br>
Figure 5.2 5-state process model
</p>

## Deadlock
Deadlock is a situation where two or more processes require the same resources and deny each other access, causing all involved processes to be unable to proceed and remain in a blocked state. <br><br>

For example:
- Process A is opening File 1 and requires File 2
- Process B is opening File 2 and requires File 1
- If neither of the process closes the file, neither process will be able to proceed.

## Deadlock Conditions
1. Mutual Exclusion (A resource can only be allocated to one process at one time, e.g. only one process can write to a file at one time)
2. Hold and Wait (A process can hold a resource while waiting for the allocation of other resources, e.g. A process can hold a file, while waiting for the allocation of another file)
3. No preemption (Resources cannot be remove from a process holding them, e.g halting of a process is not allowed)
4. Circular Wait (Set of processes waiting for each other in a circular fashion)

<p align="center">
<img width="322" height="327" alt="image" src="https://github.com/user-attachments/assets/ffeaa784-955e-40a0-b3b5-7944102b48e0" /><br>
Figure 5.3 Circular Wait
</p>

## Ways of dealing with deadlock
1. Deadlock Prevention
2. Deadlock Avoidance
3. Deadlock Detection and Recovery

**Deadlock Prevention**
There are two main ways for OS to prevent Deadlock:
1. Prevent the occurrence of one of the three conditions for deadlock to happen
2. Prevent the occurrence of circular wait

- **Mutual Exclusion** - Not possible to prevent this as some resources must be accessed by only one process at one time. (E.g if OS allows two processes to write to the same file at the same time, it may result in a corruption of the file. Some hardware resources such as printer can only be used by one process at one time.)
- **Hold and Wait** - Possible to prevent by requiring one process  to request all its required resources at one time. The procees will be blocked until all resources are available
- **No preemption** - Possible to prevent by requiring that a process that holds some resources to release its resources if needed by another process
- **Circular Wait** - Can be prevented by defining a linear ordering of resource type

**Deadlock Avoidance**
OS allows the three of the conditions to occure but it ensures that the fourth condition or rather Circular Wait never to occur, so that the deadlock point is never reached. <br>
Two approaches to deadlock avoidance:
1. Process will not be started if its demand may lead to a deadlock later.
2. Process will not be granted an incremental resource request if the allocation may lead to a deadlock later.




































































































