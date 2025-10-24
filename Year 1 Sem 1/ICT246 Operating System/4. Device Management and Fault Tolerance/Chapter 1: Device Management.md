## I/O Devices
- I/O devices interact with the computer system
- Consists of both input and output devices
- Usually, the main difference between the devices are the data rate, application, complexity of control, unit of transfer, data representation and error condition.

### Techniques used for performing I/O
- Programmed I/O
  - CPU issues an I/O command to an I/O module for a process, and then the process will be busy waiting for the I/O operation to complete
  - However, it is not efficient as the I/O operation needs to be completed before the process can continue
- Interrupt-driven I/O
  - Employ Interrupts
  - Increses Efficiency as CPU do not need to wait for the I/O operation to complete before continuing
- Direct Memory Access (DMA)
  - DMA module controls the exchange of data between the I/O module and the main memory.
  - CPU will send request to the DMA module, and the CPU will only be interrupted after the entire block has been transferred.
  - Greatly increases the efficiency (CPU is only involved at the beginning and at the end of the transfer)

## Disk
- Disk is one of the most important devices that computer communicates with
- Both the traditional hard disk and Solid-State Disk (SSD) are widely used in computers

## Disk performance parameters
- A traditional hard disk consists of platters that rotate under the read/write head.
  - E.g Laptop disks have the speed of 5400 rpm (rotational speed) or 7200 rpm. Servers can be higher with rpm such as 10K or 15K rpm.
- To read a sector in the disk, the read/write head will need to be positioned at the right track and at the start of the right sector.
  - **Seek time**: Time taken to position the read/write head on the right track
  - **Rotational delay**: Time taken to position the read/write head at the start of the right sector
- The transfer time can be represented as follows:
  - T = b/rN
  - T = Transfer time
  - b = number of bytes to be transferred
  - N = Number of bytes on a track
  - r = rotational speed, in revolutions per second (rps). Rpm stands for revolutions per minute. To get seconds, we need to divide by 60
- Total average time, Ta = Ts+1/(2r) + b/(rN)
  - Ts = average seek time
- Example exercise: <br>
A disk is having an average seek time of 4ms, a rotational speed of 7,500 rpm, and 500 sectors per track with each sector having 512 bytes. Calculate the total time to read a file with 500 sectors. <br><br>
T = 500x512/(7500/60)x(512x500) <br>
T = 256000/125x256000 <br>
T = 256000/3200 0000 <br>
T = 1/1250 = 0.008 = 8ms<br>

Ts = 0.008/2 = 0.004<br>

Ta = 0.004+1/(2x(7500/60))+0.008<br>
Ta = 0.016s = 16ms































