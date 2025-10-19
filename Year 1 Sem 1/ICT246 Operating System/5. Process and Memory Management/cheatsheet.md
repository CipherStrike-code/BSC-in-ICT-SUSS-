## Process Management
Process is a running program. When an application programs is created, process are created and ran. Process contatins the program code and a set of data.

**2-state process model**
- Running
- Not Runnning

**5-state process model**
1. New (Process created but not added into pool of executable processes)
2. Ready (Process given the resources and waiting for CPU time to execute)
3. Running (Process that is currently being executed by the CPU)
4. Blocked (Process that is temporarily halted until the resources becomes available)
5. Exit (Process has finish execution)

<p align="center">
<img width="1167" height="475" alt="image" src="https://github.com/user-attachments/assets/d3355db4-1d60-4e43-a18d-5f620df7c473" />
</p>

## Deadlock 
Situation where two or more processes sharing same resources are preventing each other from access the resources, causing all processes involved to be in a permanent block state.

**Deadlock Conditions**
- Mutual Exclusion (Each resource can only be used by one process at a single time. E.g Writing to a file)
- Hold and Wait (A process can hold onto a resources while waiting for the rest of the resources to be ready)
- No preemption (Resource cannot be removed from a process holding it. E.g Halting of a process is not allowed)
- Circular Wait (Set of processes waiting for each other in a circular fashion)

 **Deadlock Strategies**
1. Deadlock Prevention
2. Deadlock Avoidance
3. Deadlock Detection and Recovery

**Deadlock Prevention**
Two main ways:
1. Prevent the occurence of one of the three conditions for deadlock to happen
2. Prevent the occurence of circular wait

- Mutual Exclusion (Not possible as some resource needs to have this characteristic such as hardware. E.g printer and files)
- Hold and Wait (Possible by requiring the process to request all the resources at once.)
- No preemption (Possible by requiring a process that holds some resources to release its resources if needed by another process)
- Circular Wait (Can be prevented by defining a linear ordering of resource type)

**Deadlock Avoidance**
- OS allows the three conditions to occur, but the OS ensures that the deadlock point is never reached. This is done by stopping preventing Circular Wait
Two approaches to a deadlock avoidance:
1. Process will not be started if its demands may lead to a deadlock later.
2. Process is not granted an incremental resource request if the allocation may lead to deadlock later. 

**Deadlock Detection and Recovery**
- OS will check for deadlock periodically
- Once deadlock is detected, the OS can then use a strategy to resolve the deadlock. (e.gtol abort and restart al deadlocked processes)

## Processor Scheduling
Main objective of short-term scheduling is to optimise the allocation of the processor time. Important as it determines which process wil be executed by the processor. 

- First Come First Served (FCFS)
  - A process will join the ready queue once it is ready
  - When the current process stops executing, the process that has been in the ready queue longest will execute next.
- Round robin (RR)
  - An algorithm that implements the technique of time slicing
  - Each process will run for fixed amount of time, and the current executing process will be placed on the ready queue if it has utilised its time slice.
  - The next ready process is selected based on FCFS
- Shortest Process Next (SPN)
  - Non-preemptive algorithm that selects the process with the shortest expected processing time.
- Shortest Remaining Time (SRT)
  - Preemptive version of SPN
  - It will select the process that has the shortest expected remaining time. 

## Example
<p align="center">
<img width="400" height="400" alt="image" src="https://github.com/user-attachments/assets/7f3bde64-755e-4d37-bc73-9b94d50c7d77" />
<img width="400" height="400" alt="image" src="https://github.com/user-attachments/assets/9ce996dc-469b-49b8-b6d0-3e6f3d574520" />
<img width="400" height="400" alt="image" src="https://github.com/user-attachments/assets/d738ab5a-a8f0-46e1-ad5e-0fec0980c397" />
</p>

##Memory Partitioning
Main operation of memory management is to bring processes into main memory (e.g RAM) for execution
Dynamic Partitioning
- Allocates the process exactly the memory that it requires
- Can create many holes in the memory as time goes by.
- Memory will become fragemented from the holes known as external fragmentation
- Compaction can be used to solve fragmentation, but is time consuming and wasting processor time
<p align="center">
<img width="766" height="748" alt="image" src="https://github.com/user-attachments/assets/800edb9a-f2f5-4d25-b790-15623da65ead" />
</p>

OS will decide on where to swap the process into memory to minimise the holes created. 
Three placement algorithms:
1. Best-fit
   - Selects the free block closest in size
   - Usually is worst in term of performance (result in very small holes)
3. First-fit
   - Selects the first available block that is large enough from the beginning of memory
   - Usually the fastest, and the best
5. Next-fit
   - Selects the free block that is large enough from the last placement location of the memory
   - Usually performs slightly worse than the first-fit

<p align="center">
<img width="771" height="823" alt="image" src="https://github.com/user-attachments/assets/8c4af8e9-b881-48b6-b5ce-8fa68b123e11" />
</p>

## Paging 
- Used to overcome the memory fragmentation problem in dynamic partitioning
- Divides memory and process into equal fixed-size chunks that are relatively small
- Chunks of a process, also known as pages, can be allocated into chunks of a memory, which are called frames
- One page can fit into one frame






















