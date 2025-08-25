# Introduction to Virtualisation 
## What is virtualisation? <br>
Virtualisation means we are creating a virtual version of a device or resource, and that device or resource can be an operating system or even a network. Therefore, virtualisation can mean different things to different professionals.

## What is a virtual machine? <br>
A virtual machine is a machine installed with virtualisation software that can run several similar or different os. The machine that is installed with the virtualisaion software is called the host machine. A virtualisation software is usually installed inside of a host OS. A virtualisation work by utilising a software called **hypervisor**. A hypervisor sits between the hardware and the VM, and manages the resouces. Below in figure 2.1, a virtualisation layer is shown.

<p align="center">
  <img width="518" height="626" alt="image" src="https://github.com/user-attachments/assets/92a15efa-133e-4f75-899a-ad6ffb6459b7" /><br>
  Figure 2.1
</p>

Each virtual machine will run an OS, and we call the machine inside the virtual machine as guest OS. The machine running the hypervisor is called the host machine. Hypervisor are software such as virtualbox and Vmware Workstation. <br>

Below are some reasons why a company or people would use a hypervisor. 
- Consolidation (A server can run multiple VM and thus improves its efficiency by sharing its resources (such as processor, RAM, etc).
- Rapid development (A new VM can be deployed in a ver short amount of time and is easy to copy as VM consists of files.)
- Ease of management (VM facilitates deployment, and software can be tested easily. Virtualisation is one of the technologies that support cloud computing, and many of the data centres in the world are now using virtual machines.)

## Characteristic of a Virtual Machine
- It is a software that has the characteristics of how a physical machine works.
- It is configured with the necessary hardware, such as processor, RAM, storage space and network interfaces.
- It is only able to see the resources that are allocated to it (such as amount of processor core, ram and network interfaces) but not the full resources that the host machine is having.
- Consists of several files, with a configuration file that describes the attributes of the VM usually. Example will be configuration file with the extension of **.vbox** in VirtualBox and the actual OS file with the extension of **.vdi**. Vmware workstation configuration file will contain the extionsion of **.vmx**, with the actual OS file containing the extension of **.vmdk**.
- Much faster to backup and restore as compared to a physical machine as it contains only files.

# Different types of virtualisation
Hypervisor is a middle man between the guest OS and the physical host machine. There are a total of two types of hypervisors. They are type 1 and type 2 hypervisors. Below is an image (Figure 2.2) of the types of hypervisors. 

<p align="center">
  <img width="942" height="457" alt="image" src="https://github.com/user-attachments/assets/6aadcc7c-e2ef-4d04-b015-11b600ae33b5" /><br>
  Figure 2.2
</p>

## Type 1 Hypervisor (Bare-Metal)
Type 1 Hypervisor can directly control the hardware such as processor and RAM. It allows VM to be installed on it directly. Type 1 hypervisor usually has good performance as it eliminates one additional layer. Examples of Type 1 hypervisors are VMware ESXI, and Microsoft Hyper-V.

## Type 2 Hypervisor (Hosted)
Type 2 Hypervisors is installed as a software and sits above the Host operating System. The type 2 hypervisor need to go throug the Host OS to talk to the hardware. Type 2 hypervisor usually has lesser performance as compared to the type 1 hyperviosr. Examples of Type 2 Hypervisors are Oracle VM VirtualBox and VMware Workstation. 






































