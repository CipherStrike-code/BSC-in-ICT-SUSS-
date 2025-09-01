<p align="center">
  <img width="600" height="400" alt="image" src="https://github.com/user-attachments/assets/74a331a5-a634-4702-b67b-5b531f09b52b" /><br>
  Figure 2.2.1
</p>

## Processing by CPU
- CPU Operation
- Instruction set and format
- Clock rate
- Registers
- Word Size
- Performance Enhancement
- Physical Implementation
- Future Trends

## Central Processing Unit (CPU)
- CPU is also known as the computer system "brain".
- Executes program instructions including computation, comparison, and branching
- Directs all computer system actions including processing, storage, input/output, and data movement

## CPU Components
- Control Unit (Directs flow of data to/from memory, registers and the arithmeic logic unit. Access programs instructions and executes them or directs the ALU to executs them)
- Arithmetic logic unit (ALU) (Executes computation and comparison instructions)
- Registers (Storage locations within the CPU that hold ALU inputs, ALU outputs, and other data for fast access)

<p align="center">
  <img width="531" height="377" alt="image" src="https://github.com/user-attachments/assets/48540ed9-7e32-4b12-aba3-653a9d78b9da" /><br>
  Figure 2.2.2
</p>

## Instruction Cycles
An instruction cycle is also known as the fetch-execute cycle. It is needed as it provides an organised, repeatable process for the CPU to fetch, decode and execute instructions, ensuring that every program runs correctly and efficiently from start to finish. 
Three Steps:
- Fetch
- Decode
- Execute

<p align="center">
  <img width="657" height="163" alt="image" src="https://github.com/user-attachments/assets/c35911c2-644a-4acc-acab-9a2e38892670" /><br>
  Figure 2.2.3
</p>

## Fetch, Decode and Execution Cycle
The CPU constantly alternates between 3 stages (or cycles):
- Fetch Cycle:
  - The control unit reads an instruction from primary storage(RAM).
  - The control unit increments the program counter (PC), also known as the instruction pointer (address of the nexte instruction to be read).
  - The control unit stores the instruction in the instruction register (IR).
  - If there are data inputs embedded in the instruction, they are loaded into registers as inputs for the ALU.
  - If the instruction includes memory addresses of data inputs, they're copied from memory and loaded into registers as inputs for the ALU.

- Decoding Cycle
  - The Control Unit deciphers what the instruction stored in the IR means.
  - Instructions are decoded into a series of control signal that are used to execute the instruction.
  - The instructions are splited into 2 parts:
    1. Opcode (Tells the CPU what action to perform, like a command or instruction name, for example "ADD" to add numbers or "LOAD" to load data)
    2. Operand (Tells the CPU where to find the data or what data to use for the instrucion. It could be a memory address, register, or an actual value)
  
- Execution Cycle
  - Data movement instrucitons are executed by the control unit
  - Computation and comparison instructions are executed by the ALU in response to a control signal from the control unit. Data inputs flow from registers thorugh processing circuitry and the output(s) flows to one or more registers.

<p align="center">
  <img width="529" height="480" alt="image" src="https://github.com/user-attachments/assets/8cb43d8e-1fd7-4eb2-bdd5-73a626811163" /><br>
  Figure 2.2.4
</p>

## Instruction Format
An instruction is a command to the CPU to perform a single processing function on specific data inputs.
  - It is stored in the memory or a register.
  - It must be decoded to extract the processing function and data inputs
  - Instruction Components:
    - Opcode (Unique binary number representing the procesing fucntion and a template for extracting the operands
    - Operands (One or more groups of bits after the op code that contain data to be processed or identify the location of that data (A register or a memory address))
  - Different kinds of operands have different lengths based on the type of data or address stored
  - Same processing function may correspond to many different op-codes with different operand formats (e.gg, and ADD instruction for intergers stored as operands, another for integers stored in registers, and another for intergers stored in memory)

<p align="center">
  <img width="495" height="186" alt="image" src="https://github.com/user-attachments/assets/4b282000-4a0e-4440-abd6-6084a3b65dbe" /><br>
  Figure 2.2.4
</p>

## Clock Rate
The system clock is a digital circuit that generates timing pulses, and transmits the pulses to other devices in the computer
- It is generally a seperate device with a dedicated communication line monitored by all devices in the computer system.
- All actions, especially the CPU's fetch and execute cycles, are timed according to this clock.
- Storage and I/O devices are timed by the clock signal
- All devices in a computer system coordinate their activities with the system clock

The system clock generates "ticks" at regular intervals:
  - Each tick of the clock begins a new clock cycle
  - The CPU clock rate is the frequency of those ticks
  - Typically stated in gigahertz (GHz) - billions of cycles (ticks) per second
  - Inverse of the clock rate is clock time.
  - Cycle time is the time required to fetch and execute the simplest instruction in the instruction set (e.g., NOT)
  - Cycle time = 1/Clock Rate

## Registers
Divided into two class:
  1. General Purpose
     - Used to store transient/temporay data required by the program
     - More are better up to a point (Law of Diminishing Returns)
     - Modern CPU typically provide a few dozen per ALU
  2. Special-Purpose Registers
     - 










































































