## Redundant Array of Independent Disks (RAID)
- RAID is an example of fault tolerance
- RAID uses redundant disk capacity to store parity so that it can rebuild the data in case of disk failure.
- RAID is widely implementd in servers (Hard disks used by servers are bound to failure if running long enough)

There are a total of 7 RAID level, ranging from RAID 0 to RAID 6. However, we will only talk about RAID 0, RAID 1, RAID 4, RAID 5 and RAID 6. There is also a RAID 10 but it is just RAID 1 + RAID 0

## RAID 0
- No fault Tolerance (It does not duplicate and there is no parity bits)
- Used to improve the performance and speed of the system.
- It is also known as a stripe set and data is being divided across set of drives.
<p align="center">
<img width="710" height="311" alt="image" src="https://github.com/user-attachments/assets/d269bbe3-a50b-47c7-bdf8-f527ebdbb0ca" /><br>
  Figure 4.1
</p>

## RAID 1
- It is also known as mirroring as it writes the same data on two drives.
- It does not increase performance.
- When 1 drive fails, the 2nd drive is used, and the failed drive is manually replaced. The content is then duplicated onto the new drive.
<p align="center">
<img width="1201" height="290" alt="image" src="https://github.com/user-attachments/assets/3fb1bd50-5f6c-4d81-87ec-e5011eaee493" />
  Figure 4.2
</p>

## RAID 4 
- One disk is used to store the parity bits.
- Data are divided into blocks across multiple disks with a separate, dedicated disk solely for storing parity information.
- Block-level striping and seperate parity disk are used.
- It allows up to 1 disk failure.
<p align="center">
<img width="1201" height="352" alt="image" src="https://github.com/user-attachments/assets/239dea2f-fa79-469d-8a2a-5180646e95c4" />
  Figure 4.3
</p>

## RAID 5
- Similar to RAID 4 but the parity is striped across all disks instead of using one whole disk for parity
- Requires a minimum of 3 disks.
- Generally faster than RAID 4 due to the distributed parity.
<p align="center">
<img width="1010" height="396" alt="image" src="https://github.com/user-attachments/assets/95a5db9d-a0ed-47e2-a4cd-b55ad83f853f" />
Figure 4.4
</p>

## RAID 6
- Uses two different parity calculations, and teh parity is stored across the different disks
- Allows up to 2 disk failure
<p align="center">
<img width="1160" height="325" alt="image" src="https://github.com/user-attachments/assets/4d498fa3-a84a-43ba-8c33-d4b7f6c632a8" />
Figure 4.5
</p>








