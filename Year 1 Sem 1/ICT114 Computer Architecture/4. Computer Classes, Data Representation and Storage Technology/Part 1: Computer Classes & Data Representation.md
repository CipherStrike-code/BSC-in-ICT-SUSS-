## Computer Classes and Types
| Class | Subclasses | Description |
| --- | --- | --- |
| **Personal Computing Devices** | Workstations, Laptops, Tablets, Smartphones | Meets the needs of one user at a time. <br> **Workstations** are desktop computers – ordinary or “high-end”. <br> **High-end:** <br> • Greater CPU power, more memory, better graphics, and/or faster secondary storage. <br> • Customized for very demanding single-user tasks such as video editing, animation, and computer-aided design. |
| **Smart Devices** | Appliances, Phones, Power Tools, Televisions, Vehicles, and more | Small computers embedded in a wide variety of devices. |
| **Servers** | Midrange Computer | • Supports up to several dozen simultaneous users in one or more modes: <br> - Sharing a resource via a network (e.g. email messages/folders, a database, or a website). <br> - Multiple directly-attached video display terminals (e.g. Citrix). <br> - Virtual computing – hosting multiple “virtual” microcomputers. <br><br> **Typical subsystem capabilities:** <br> - 1–16 CPUs <br> - 1–8 GB memory per CPU <br> - Large, fast, fault-tolerant secondary storage subsystem <br> - Embedded or directly-connected secondary storage backup <br> - Multiple high-speed network connections <br> - Redundant power supplies <br><br> Can also be used as a building block for larger computers. |
| **Servers** | Mainframe Computer | Supports large numbers of simultaneous users and programs: <br> - Dozens of CPUs <br> - Memory to match the number of CPUs <br> - Sustained data transfer rates among primary and secondary storage measured in hundreds of MB/s or GB/s <br> - Sustained data transfer to/from networks measured in tens of gigabits per second <br> - Ability to manage and utilize terabytes of data. |
| **Servers** | Supercomputer | **Primary purpose:** Perform as many calculations as possible in as short a time as possible. <br> Other high-end capabilities (e.g. memory size and speed) are secondary to computational performance. <br><br> **Typical specs:** <br> - Hundreds to hundreds of thousands of CPUs performing trillions to quadrillions of calculations per second. <br> - Modular architecture: <br> • All CPUs working on one big problem, or <br> • CPU subsets assigned to separate problems. |

## Server 
A computer system that manages one or more shared resources such as file systems, databases and websites. It makes these resources available to other computers using a network. A server is not a hardware type but a mode of use. Every computer can be configured to be a server by providing service to other computers over a network. However, no computer is a server inherently by default. 

- The hardware class required to implement a server depends on the type of service, resources and the number of simultaneuous users.
  - Personal Blog (Any old computer)
  - 1 Terabyte database for 1000 users (Mid Range computers)
  - E-commerce website (Mainframe or cluster of mid range computers)
  - Weather Forecasting (Super computer for computations with data storage managed by mainframes and/or midrange computers)
 
## Multicomputer Configurations
- Any arrangement of multiple computers to support a specific set of services or applications.
- Common multicomputer configurations:
  1. Cluster
  2. Blade
  3. Grid
  4. Cloud

## Cluster Configuration
- Multiple similar or identical comptuers connected by high-speed network in a dedicated configuration
- Uses architectural technique such as redundancy/parallelism, specialisation, or both, to simulate a larger-capacity computer and run a single application
- Typically placed close to each other
- Advantages: Scalability and Fault Tolerance
- Disadvantages: Complex configuration and administration

## Blade Configuration
- A cluster housed in one cabinet, a specialised cluster
- Blades are circuit boards that contain most of a computer system (Limited secondary storage adn I/O)
- Advantages: Scalability, Fault Tolerance, Simpler to modify, Concentrate more computing power in less space
- Disadvantages: Complex configuration and administration

## Grid Configuration
- Distributed architecture that combines computer resources from different locations to achieve a common goal. Task is divided into smaller subtasks and executed concurrently across multiple systems
- Computers work cooperatively at some time and independently at others
- Tends to use "ordinary" network connections not dedicated to the grid since computers may be widely dispersed.
- Computers can be located in separate rooms, buildings, or continents.
- Advantages: Scalability, Efficient Resource Utilisation, Complex Problem Solving, Collaboration, Cost Saving, Parallel Processing.
- Disadvantages: Security Risks, Limited Flexibility, Complex Configuration and Administration

## Cloud Configuration
- An extension of the grid concept
- Users interact with a front-end system which in turn musters whatever grid resources are needed
- Clouds typically employ virtualisation, allowing resources to be created and made available on demand.
- Clouds maintain resources such as storage and websites on behalf of users, the resources are permanenetly located "outside" the suign organisation.

## CPU Data Types
There are a total of 5 data types that a CPU can manipulate directly. 
1. Integer
2. Real Number
3. Character
4. Boolean
5. Memory Address

CPU can also implement multiple versions of each type to support different types of processing operations. For example, for the type integer, it supports 8-bit, 16-bit, 32-bit and 64-bit and for character it supports 8-bit (ASCII), 16-bit (Unicode) and 32-bit (UTF-32).




































































































