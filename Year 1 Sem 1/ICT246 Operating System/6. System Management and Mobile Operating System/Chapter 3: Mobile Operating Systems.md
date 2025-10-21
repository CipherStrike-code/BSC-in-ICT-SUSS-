## Mobile Operating System
- Andoid Operating System is also known as Mobile OS.
- Mobile OS has a different objective to fulfil as compared to its desktop counterpart.
- Mobile Devices are typically bulld towards a smaller screens, having constant access to cellular network, less memory and storage space compared to its desktop counterpart.
- It is not build to cater to multi user. Adding devices to the machine is not critical. It is important to extend the device battery life.

## Android Operating System
- Android OS is Open Source. It is designed for mobile phone and is based on Linux.
- Android OS currently is the most widely used mobile OS.
- Besides being the most popular mobile OS, it is also used widely in Internet of Things (IOT)

## Android Architecture
<p align="center">
<img width="500" height="450" alt="image" src="https://github.com/user-attachments/assets/680cf83e-9702-4e48-ace8-edc28e30ac3b" /><br>
Figure 6.1 Android Software Architecture
</p>

## Application Layer
- Users interact directly with the applications in the applications layer
- There is usually a core set of applications such as Contacts, E-mail, sms, browser, and so on
- Java is a common language to implement the various applications

## Application Framework Layer
- High-level building blocks are providied to the programmers, such that the reusability of components is encouraged
- The framework such as activity manager, window manager, telephony manager, and resource manager makes the job of the developers easier.
- Standardisation can be enhanced using Application Programming Interface (API)

## System Libraries
- Consists of useful system functions
- Written typically in C/C++
- Called from the application framework via a Java interface
- Surface manager, OpenGl, Media Framework, SQL Database, and Browser Engine are some of the important system libraries that the developers can use.

## Android Runtime
- Android Software is not compiled directly on the hardware. It is mapped into bytecode format and then transformed into native instructions on the device

## Linux Kernel
- Android kernel is smaller than the standard Linux Kernel
- Drivers that are not necessary in mobile devices are taken out
- Kernel in android are customise to mobile ennvironment and not desktop environment
- Android kernel provides the usual OS features such as process management, memory management, security, etc.

## iOS
- Proprietary OS developed by Apple and used exclusively in Apple's mobile devices
- Based on Macintrosh OS X, and is initirally only used for iPhone.
- Makes use of Grand Central Dispatch (GCD), which is a multi-core support capability
- GCD make it convenient for developers to split a program into multiple threads
- Developers can develop more efficient program, and are able to utilise the multi-core capabilities of the device
- GCD enhances the parallelism of the iOs capability, allowing users to feel the phone is running smoothly despite of multiple open applications. 

## iOS vs Android OS
- iOS is generally more secured
- iOS is not easily customisable

## iOS Architecture
- Uses layered approached, similar to Android OS
<p align="center">
<img width="450" height="460" alt="image" src="https://github.com/user-attachments/assets/0631320e-8ecf-466a-b0e8-b2ab243beb54" /><br>
Figure 6.2 iOS Architecture
</p>

## Cocoa Touch 
- Application layer in iOS architecture
- Deals with frameworks for development, as well as providing API
- Developers can use both swift and C to develop iOS applications

## Media Layer
- Provides support for the frameworks that deal with media (Video, Audio and graphics)

## Core Services
- Provides Core services
- Includes frameworks such as address book, core location, etc

## Core OS
- Deals with low-level features
- Provides framework such as security services framework, etc.










































