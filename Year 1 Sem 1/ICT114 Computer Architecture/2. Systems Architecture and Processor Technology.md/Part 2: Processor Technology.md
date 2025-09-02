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
     - **Accumulator (AC)**, CPU uses this register as the default location to store any calculations performed by the ALU. It is a temporary storage location for arithmetic operations, allowing the central processing unit (CPU) to perform complex calculations. <br>
     - The following registers are used primarily by the control unit in CPU management tasks:
        - **Program Counter (PC)** - memory address for next instruction fetch, aka instruction pointer
        - **Instruction Register (IR)** - copy of most recently fetched instruction
        - **Program status word (PSW)** - Set of bit flags containing error and other codes related to processing results, for example:
            1. Result of comparison operators
            2. Divide by zero
            3. Overflow and underflow

## Word Size
A word is also known as:
  - A fixed number of bits/bytes
  - The basic "unit" of data transformation in a CPU
  - The size of a data item that the CPU manipulates when executing a "normal" instruction
  - In most architecture, it is also known as the size of a memory address.

The term "word size" has been disuse as more complex CPU designs employ/take on multiple word sizes.
- An example is where a 64-bit Intel Core CPU has word sizes ranging from 16 to 128 bits.

## Performance Enhancement Techniques
With the improvement of technology, CPU designers are able to take on more complex performance improvement techniques both individually and in combination, including:
  - Memory Caching (Will be touch in seminar 5)
  - Pipelining
  - Multiprocessing
  - Branch prediction and speculative execution

## Pipelining 
This is a Henry Ford era technique (sequential assembly) applied to executing program instructions
- Execution stages:
  1. Fetch from memory
  2.Increment and store program counter (PC)
  3. Decode instruction and store operands and instruction pointer
  4. Access ALU inputs
  5. Execute instruction within the ALU
  6. Store ALU output <br>
  
Pipelining attempts to overlatp instruction execution by performing each stage on a different instruction at the same time.<br>

**Without pipelining: 1 instruction takes 6 CPU cycles => 10 instructions take 60 CPU cycles<br>
With pipelining: 1 instruction takes 6 CPU cycles => 10 instructions take 15 CPU cycles**

<p align="center">
  <img width="2873" height="1260" alt="image" src="https://github.com/user-attachments/assets/9414d85a-bd94-4dc4-94ef-8645929a76ec" /><br>
  Figure 2.2.5 Overlapped instruction execution via pipelining
</p>

Although it sounds great in theory, pipelining do has its own complexities. For example:
 - Is one program counter enough?
 - Is one instruction register enough?
 - Is one set of general purpose registers enough?
 - Is one ALU enough?
 - What happens if a branch is encountered?

Pipelining can be "finer grained" than we've shown thus far
  - For example, execution (usually the longest stage) could be (and is often is) further subdivided into additional stages

## Multiprocessing
- Pipelining goes hand-in-hand with at least some duplication of processor circuitry
- Multiprocessing carries the duplication to higher levels, such as:
  - Multiple ALUs (with parallel execution of instructions) per CPU (common by late 1990s)
  - Multiple CPUs on a single motherboard (common by early 2000s)
  - Multiple CPUs on a single chip (Common by late 2000s)
 - Modern Operating systems are more complex because they now manage more processing resources and complex application software
 - Application software that takes advantage of multiprocessing is more complex because it must be designed for parallel execution (aka multithreading)

## Branch Prediction and Speculative Execution
- Branches cause problems with pipelining as they invalidate the partially executed instructions that follow them:
  - Wrong instructions (after the branch) were fetched and partially executed
  - Special and general purpose register contents are incorrect
- Pipeline must be flushed and filling it with the proper set of instructions (the branch target) must be anew
- Real programs have lots of branches
  - Thus, pipelining will often "fail" unless preventive measures are employed.

## Branch Prediction and Speculative Execution Preventive Measures
- **Look Ahead** - "watch" incoming instructions for branches and alter standard behavior accordingly
- **Branch prediction** - the CPU guesses whether a branch condition will be true or false based on past experience
  - If the guesses are right most of the time, the processor can prefetch the correct instructions and buffer them so the processor is kept busy
- **Speculative Execution**
  - As the CPU executes conditional BRANCH instructions, it keeps score how often the condition for each branch instruction has been true or false
  - Based on the scores, the CPU speculatively execute instructions ahead of their actual appearance in the execution, holding the results in temporary locations
  - This enables the processor to keep its execution engines as busy as possible by executing instructions that are likely to be needed
- Speculatively execute both paths beyond a conditional branch
  - Requires multiple execution units
  - Half the results will be thrown away (half the effort is wasted)

Modern CPUs employ all three techniques to improve pipelining performance






































































