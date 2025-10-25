## Memory Partitioning 
- Main operation of memory management is to bring processes into main memory (e.g. RAM) for execution
- Dynamic Partitioning
  - It is a method that allocates the process exactly the memory that it requires
<p align="center">
<img width="500" height="400" alt="image" src="https://github.com/user-attachments/assets/9d6a468c-39dc-4aec-af9d-753578bd3d84" />
</p>
Dynamic partitioning is good, but it will create many small holes as time goes by. This causes the memory to be fragmented, and is known as external fragmentation. <br>
Compaction can be used to solve the issue, but it is time consuming and waste processor time. <br><br>

Since memory compaction is time consuming, the OS will need to decided where to swap the process into the memory to minimise the holes created. There are 3 main placement algorithms:
1. Best-fit
   - Selects the free block that is closest in size
   - Usually is the worst in terms of performance. It has to search through all available memory holes to find the smallest one that fits. The tighest spot is always bit, result in tiny leftover space that are often too small to fit future processes.
3. First-fit
   - Selects the first available block that is large enough from the beginning of memory.
   - Usually the fastest and the best
5. Next-fit
   - Selects the free block that is large enough from the last placement location of the memory
   - Usually performs slightly worse than the first-fit
   
<div align="center">
  
| Algorithm | Search Time (Speed) | Fragmentation | Overall Performance |
|---|---|---|---|
| First Fit | Fastest | Moderate | Best Balance |
| Next Fit | Fast | Slightly more fragmentation | Good |
| Best Fit | Slowest | Highest fragmentation | Worst |
  
<img width="400" height="300" alt="image" src="https://github.com/user-attachments/assets/4c46df32-c351-42e7-81e9-b7972b531f2b" />
</div>

## Paging
- Paging is used to overcome the memory fragmentation problem in dynamic partitioning
- It divides memory and process into equal fixed-sized chunks that are relatively small
- Chunks of a process, called pages, can be allocated into chunks of a memory, which are called frames
- One page can fit into one frame

<p align="center">
<img width="400" height="300" alt="image" src="https://github.com/user-attachments/assets/5e945014-7b01-49e5-a8b8-c61f9d3cf332" />
<img width="400" height="300" alt="image" src="https://github.com/user-attachments/assets/3b748e63-7cac-4018-bf4b-4627ac1c9a69" />
</p>


































