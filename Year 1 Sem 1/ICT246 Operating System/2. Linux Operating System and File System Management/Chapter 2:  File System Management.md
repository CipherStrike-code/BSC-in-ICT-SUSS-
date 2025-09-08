## Overview of Files and File Systems
File Desirable Properties:
- Long-term existence
- Sharable between processes
- Can be organised into a hierarchical structure

File Systems:
- Provide a collection of functions and operations that can be performed on files
- E.g. Create, Delete, Close, Read and Write

File Management Systems:
- A system software that provides file usage services to applications and users.
- Relieves the developers to develop file access functions for each application
- Meets the user requirement such as data storage, perform file operation

## File System Software Architecture
<p align="center">
  <img width="557" height="368" alt="image" src="https://github.com/user-attachments/assets/0f8b22d6-1733-4e0a-a389-789ecd68df23" /> <br>
  Figure 2.1
</p>

## Parts of the File System Software Architecture
**Disk Device Driver/Tape Device Driver**
- Responsible for communication with the disk and tape.

**Basic File System (I/O)**
- Deals with blocks of data that are exchanged with disk/tape
- Does not understand the file content

**Basic I/O Supervisor**
- Deals with device I/O, scheduling and file status
- Selects the device based on the particular file selected

**Logical I/O**
- Maintains basic data about files























