## Introduction to Virtualisation
<p align="center">
  <img width="399" height="388" alt="image" src="https://github.com/user-attachments/assets/54f1a49c-ac31-4406-846c-cc8be6b911a3" /><br>
  Figure 1.1 Virtualisation Stack
</p>

**What are hypervisors?**
Hypervisors are software that enables multiple operating machines (VMs) to run on a single physical system. They allocate and manage the computing resources needed by each virtual machine (VM), enabling efficieny, flexibility and scalability.

**What are virtual machine?**
A Virtual Machine(VM) is a operating system running on top of a host system, enabled by a hypervisor. It allows muliple operating system to run on one physical system. Each VM is isolated and can only access to the resources allocated to it.

## Benefits of using hypervisor
1. Consolidation
   - A server can run multiple virtual machine and improves its effiency by sharing its resources.
2. Rapid Deployment
   - A VM can be deployed in a very short time span as VMs consist only of files. This also makes it easy to copy, transfer, and back up.
3. Ease of Management
   - VM facilitates deployment, and software can be tested easily. Virtualisation now is widely used in data centers, as it supports cloud computing.

Types of hypervisors:
1. Type 1 Hypervisor (Bare Metal)
   - Sits directly on top of hardware
   - Allows direct control of hardware such as RAM and processor
   - Good Performance as one layer is removed.
   - Examples are VMware ESXi and Microsoft Hyper-V 
2. Type 2 Hypervisor (Hosted)
   - Sits on top of the host operating system
   - Needs to go through Host OS to talk to the hardware
   - Has less performance than Type 1 hypervisor
   - Examples are Vmware Workstation and Oracle Virtual Box

## Operating System Booting Process
Steps:
1. Processor execute bootstrap program from Basic Input/Output System (BIOS). (First Stage boot-loader)
2. Boot loader executes code from boot block stored in hard drive.
3. Code from boot block start OS.

1. POST (hardware check)
2. Bootloader loads
3.Kernel loads into memory
4. Kernel initializes hardware + system functions
5. OS services start
6. User interface provided






















