## Overview of Files and File Systems

### File Desirable Properties
- Long-term existence
- Sharable between processes
- Can be organised into a hierarchical structure

### File Systems
- Provide a collection of functions and operations that can be performed on files
- Examples: Create, Delete, Close, Read, Write

### File Management Systems
- System software that provides file usage services to applications and users
- Relieves developers from implementing file access functions for each application
- Meets user requirements such as data storage and performing file operations

---

## File System Software Architecture

<p align="center">
  <img width="557" height="368" alt="image" src="https://github.com/user-attachments/assets/0f8b22d6-1733-4e0a-a389-789ecd68df23" /> <br>
  <em>Figure 2.1: File System Software Architecture</em>
</p>

---

## Parts of the File System Software Architecture

**Disk Device Driver / Tape Device Driver**
- Responsible for communication with the disk and tape

**Basic File System (I/O)**
- Deals with blocks of data that are exchanged with disk/tape
- Does not understand the file content

**Basic I/O Supervisor**
- Deals with device I/O, scheduling, and file status
- Selects the device based on the file being accessed

**Logical I/O**
- Maintains basic data about files

---

## File Directories
- Tree-structured directory is popular (Windows, Linux)
- Windows uses drive letters (e.g. `C:\\drive`)
- Linux file structure starts with the root folder `/`

### Types of Path
1. **Absolute Path**
   - Full path that points to the same location regardless of the current working directory
2. **Relative Path**
   - Starts from the current working directory, so the full path does not need to be provided

---

## File Allocation Methods
A file consists of a collection of blocks on secondary storage (e.g. hard drive).  
One of the main functions of the OS is to allocate blocks to files, handled by file system management.

### 1. Contiguous Allocation
- Includes Start Block and Length
- Each file occupies a contiguous set of blocks on the disk

<p align="center">
  <img width="628" height="422" alt="Contiguous Allocation" src="https://github.com/user-attachments/assets/2573a9af-b6fc-4136-a9d6-40193a47dc79" /> <br>
  <em>Figure 2.2: Contiguous Allocation</em>
</p>

| Advantages | Disadvantages|
| --- | --- |
| Very Fast Sequential and random access since number of seeks are minimal | External Fragmentation making inefficient usage of memory|
| Simple to implement | Hard to grow files as it depends on the availability of contiguous memory at a particular instance |


---

### 2. Chained Allocation (Linked List Allocation)
- Each file is a linked list of disk blocks (not necessarily contiguous)
- Each block contains a pointer to the next block in the file
- Only the first block address is stored in the directory

<p align="center">
  <img width="562" height="432" alt="Chained Allocation" src="https://github.com/user-attachments/assets/ccecfbc6-26aa-4ac6-8fdb-2e68c7173a22" /> <br>
  <em>Figure 2.3: Chained Allocation</em>
</p>

---

### 3. Indexed Allocation
- Each file has an **index block** that contains a list of all block addresses
- The index block allows direct access to any block of the file
- Blocks do not need to be contiguous and can be scattered on disk

<p align="center">
  <img width="562" height="432" alt="Indexed Allocation" src="https://github.com/user-attachments/assets/c0e5b9b4-ab65-461c-930b-1b8a460f208c" /> <br>
  <em>Figure 2.4: Indexed Allocation</em>
</p>

---
