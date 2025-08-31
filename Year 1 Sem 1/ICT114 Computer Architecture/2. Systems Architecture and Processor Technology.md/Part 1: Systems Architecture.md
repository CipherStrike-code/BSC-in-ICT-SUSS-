## Computer Capabilities
- **Processing** (Done by processor) 
  - Perform computations
  - Perform logic functions such as comparison and branching
- **Storage** 
  - Able to store instructions and data
- **Communication** 
  - Within itself and with other devices

## Computer Processors 
There are a total of 2 types of processors. 
1. **General-Purpose Processor** (General purpose processor, Microprocessor, Von Neumann processor)
    - Reads its program instructions from a **storage device** (Example. Hard disk, Memory)
    - Contents of the storage device are changeable, so the program and the function performed by the processor can change.
2. **Special-Purpose Processor** (Embedded processor, Application-Specific processor, Application-Specific Integrated Circuit (ASIC), GPU)
    - Uses program storage that can't be altered
    - Has a single program "wired" into the processor
  
**Note:** Both **General-Purpose Processor** and **Special-Purpose Processor** share the same characteristics as they are both processors.

## Processor Characteristics and Functions

- A processor should be able to perform the following functions:
    - Arithmetic Computation (+, -, x, ÷)
    - Comparison (<, =, >, ≠, ≤, ≥)
    - Data movement and communication among memory, mass storage, and I/O devices
 - Perform instruction given by the memory
    - Memory → Processor → Execution → Output

## Instruction 
- A command to the processor to perform a specific function (e.g., arithmetic operation) on specific data.
- Each instruction is relatively simple.
- Complex tasks are accomplished by combining many instructions into a program and executing the program.
- When a processor “follows an instruction,” it is said to be executing the instruction.
- An instruction is a command to a processor to let the processor to know to perform specific functions.

**Storage Capacity**
Computers need to be able to store:
  - **Intermediate processing results** (Also knowns as a temporary output at a certain stage of the process or workflow, which may be used for further operations or as an input for a later stage)
  - **Data** (Persistent Output from a previous program execution and can be used as input for future executions. It is different from intermediate processing result as it is not temporary and can be used in different process or workflow.)<br>

<div align="center">

| Aspect	| Intermediate Result	| Output Data (Past Executions) |
| --- | --- | --- |
| Stage	| During processing	| After processing |
| Persistence	| Temporary	| Permanent/Stored |
| Purpose	| Used for next steps	| Used for future program input |
| Example	| Partial sum in calculation	| Saved report in a database |

</div>
  -  Programs

There are however several differences between storage devices and these characteristic are:
- Speed
- Volatility
- Cost per bit

## Input/Output Capability
I/O devices must be able to comprise many communication modes:
- Sound, text and graphics for human interaction
- Electronic or optical communcation for other computers interaction

## Computer Hardware
There are 4 major functions of computer hardware. They are:
- External Communication
- Storage
- Processing
- Internal Communication

## Hardware Components
4 Main Components make up a Computer System
1. CPU
2. Main Memory
3. I/O Unit
4. System Bus

| Components | Functions |
| --- | --- |
| CPU | A Processor that performs computation, comparison and data movement |
| Main Memory | It is also known as primary storage. It is used to store both data and instructions |
| I/O Unit | Performs exterenal communication functions |
| System Bus | A communication channel taht connects all the computer system. It includes the data bus, address bus, and control bus that carry data, memory addresses, and control signals respectively. The system bus acts like a communication highway within the motherboard enabling data transfer and coordination between components.|

<p align ="center">
  <img width="556" height="367" alt="image" src="https://github.com/user-attachments/assets/c733ab40-a72d-4625-806a-789cd2d1c62b" /><br>
  Figure 2.1.1
</p>

## Central Processing Unit (CPU)
- A CPU is a general-purpose processor that executes instructions.
- It is implemented on microprocessor "chips"
- Modern chips can have multiple CPU in a single chip
- The CPU is also considered as the computer's "brain"
- A CPU is internally divided into regions that perform specialised functions, similar to how a human brain work

## CPU Components
**Arithmetic-logic unit (ALU)**
-  Performs computation and logic instructions
**Registers**
- Internal storage locations - each holds one data item
- Hold inputs and outputs from the ALU
**Control Unit**
- Moves data among registers and other computer system storage locations
- Accesses program instructions and either executes them (data movement) or directs the ALU to execute them (computation and logic instructions).
- Manages the sequence of instructions, including branching, loops and decisions to control which instructions to execute next. (Control Flow)

A CPU has three fundamental functions:
1. Arithmetic and Logic Computations (Handle by ALU)
2. Data Movement (Movement of data between registers, memory and I/O handled by Control Unit)
3. Control Flow (Deciding the order of instruction execution handled by the Control Unit)

<p align="center">
  <img width="531" height="362" alt="image" src="https://github.com/user-attachments/assets/97acb709-f3f5-4ad6-b055-67a85c4227c0" /><br>
  Figure 2.1.2
</p>

## Primary Storage
- Computer's main memory is used to hold the operating system, system data, programs and any data currently in use.
- Volatile memory, so it will lose its content when power is off
- Accessible directly by the CPU for reading and writing
- Typically faster but smaller
- Examples of Primary Storage are: RAM, Cache, Registers

## Secondary Storage 
- Hold large quantities of data and programs
- Is non-volatile
- Much cheaper per bit than primary storage
- Much slower than primary storage
- Examples of Secondary Storage are: Magnetic disk, Optical Disk, Hard Disk Drive, Solid State Drive and Magnetic tape

**Storage Comparison** 

| Type | Implementation | Content | Typical quantity |
| --- | --- | ---| --- |
| CPU Registers | High-speed electrical devices implemented within the CPU | Currently executing instruction(s) and associated data inputs and outputs | Several dozen to a few hundred per CPU |
| Primary storage | High-speed electrical devices (RAM) implemented outside but close to the CPU | Current programs and immediately needed data to the extent it will fit | 1-8 billion data items per CPU |
| Secondary Storage | Low-speed electromagnetic and optical devices | Programs not currently being executed and data not currently being accessed by programs | Billions (gigabytes), trillions (terabytes), or quadrillions (exabytes) of data items |

## System Bus
- The System Bus is the communication channel that connects all devices in the computer system. 
- Bus speed is critical factor in determining the overall speed of the computer system.
- Modern computers use additional buses to improve performance.
  - Storage bus (Used to connect multiple magnetic disk drives to a single connection point on the system bus)
  - CPU Memory bus (Used for direct transfer of data between the CPU and primary storage)
  - Video bus (Used for direct transfer of data between memory and the video/graphics controller)
















































