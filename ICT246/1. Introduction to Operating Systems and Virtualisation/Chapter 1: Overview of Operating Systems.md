# Introduction to Operating System
Operating systems are an integral part of our daily life, powering mobile devices such as phones and laptops to our computers and smart television. It is essenstial that we, as Infomation and Communciation Technology (ICT) Professional, know more about Operating System (OS) than what the general public knows. 

Example of Operatings are: 
1. Android
2. iOS
3. Windows 10
4. Windows 7.

# Introduction to Computer System
A computer System can be divided into 4 componenents. Mainly, the 
1. User
2. Application (Web Browsers, Software)
3. Operating System
4. Hardware (Central Processing Unit(CPU), Memory and Input/Output (I/O) Devices)

<p align="center">
  <img width="476" height="420" alt="image" src="https://github.com/user-attachments/assets/bafb47a0-bf79-4318-a603-601400224a03" />
</p>

- A hardware provides the basic computing resources for the system.
- The applications are designed to define how computing resources are beign used to solve the user problem.
- The Operating system controls the hardware and coordinates its resources with the software, acting as a bridge between the software application and hardware.

An operating system is essential as it plays a huge part in liasing between the hardware and input devices such as the keystroke from the keyboard to the application software such as Microsoft word.

# Core Functions of an Operating System
An OS must fulfill 3 objectives. They are:
1. Convenience (Making a computer easier to use)
2. Efficiency (Making efficient use of the system resources)
3. Ability to evolve (Permits new systems to be introduced)

## Convenience - Operating System as a user/computer interface
The Operating System as a user/computer interface needs to handle the hardware for the users. Users do not care about how the hardware works but rather how the computer can help to make their work easier. OS also need to make the job of an application programmer easier by providing services that the programmer can use. Typically, OS provides services in the following areas.
- Program Execution (OS handles the execution of program and process, and schefuling of resources
- Access to I/O devices (OS handles the hardware and provides simple read/write for the different hardware devices
- Controlled access to files (OS provides file management services as well as providing mechanism of access contorl to files and folders
- System Access (OS resolves conflict for resource contention as well as control access to the system.)
- Error detection and response (OS handles varies errors conditions such as issues in executing program)
- Accounting (OS monitors performance and provides statistics for the users to view)

## Efficiency - Operating System as a resource manager
OS needs to control the use of a computer's resources, such as input devices and output devices, both main and secondary memory, and processor execution time. It is a software and needs to be executed by the processor. Thus, it needs to hand over control when necessary to other appication program, and it depends on the processor to let it regain contorl. Thus, we can treat OS as a special software as compared to application programs. 

## Ability to evolve - Ease of Evolution of an Operating System
A OS will have be able to evolve due to 
- Hardware upgrades/new types of hardware - eg. touchscreen
- New Services - eg. new management tools
- Fixes - eg. new patches (such as the Windows patches)

# Evolution of Operating Systems
We have to know the history of how OS comes about in order to know OS the best. Computers do not have an OS in the earlier days. This result in the programmer needing to interact directly with the hardware, which is tedious and not convenient. This is also known as **Serial processing** as the users accessed the computer in series. Through the years, something called batch system is developed, which is like an early version of the modern OS. The simple batch system has an OS, which means that the user do not need to directly deal with the hardware, making it more convenient to use. 

Despite the fact that the simple batch system improves the usage of the computer, it is not as efficient as the processor is often idle and not being utilised. This is because the Input/Output (I/O) devices of that time are much slower as compared to the processor. Thus, multiprogrammed bathc system is develop which improves the efficiency of the computer. 

In the figure (1.1) below, it shows a **Uniprogramming** solution where there is only one program running and thr processor will execute until it hits and I/O operation and it has to wait. However, the wait period is much longer, as the I/O is much slower as compared to the processor.

<p align="center">
  <img width="725" height="140" alt="image" src="https://github.com/user-attachments/assets/d1c5643a-9561-4d89-baf6-cf507f1d9e73" /><br>
  Figure 1.1
</p>

The figure (1.2) below shows a **Multiprogramming** situation, where there are two programs A & B. When A hits and I/O operation, program B can execute, thus improving the overall efficiency of the system.  

<p align="center">
  <img width="935" height="362" alt="image" src="https://github.com/user-attachments/assets/60fa0c8f-1988-493d-983b-213975fdfa5c" /><br>
  Figure 1.2
</p>

Although the multiprogramming batch system improves the efficiency of the processor, it does not handle interactive jobs. Thus, time-sharing system is developed, and is being used to handle multiple interactive jobs. In time-sharing system, multiple users share the processor time, and the OS interleave the execution of each user program in a short burst of time.<br>

Multiprogramming is used in both batch processing and time sharing. In batch processing, the processor usage is maximised, and Job Control Language (JCL) commands are provided with the job. Note that JCL is an old language and it is still being used in mainframe system, which is used in some large organisations in the world. In time sharing system, the response time is minimised, and commands are entered at the terminal.
 
# Major Achievements in Operating Systems
Four important core functions of operating system have advanced a lot throughout the years, creating the modern operating systems that we have now. <br>
The four important core functions or advancement are:
- Processes
- Memory Management
- Information Protection and Security
- Scheduling and resource management































