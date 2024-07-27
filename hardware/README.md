# Hardware
My solution is composed by a single board computer and two Hard Disk Drive. I was looking for a low power consume computer and a reliable solution for the data. 

# How to chose the Board
There are multiple board solutions for NAS and cloud, e.g., Raspberry Pi 4/5 or Orange Pi, and all of them are good alternatives to the ZimaBlade. I decided to buy the ZimaBlade because it exposes two SATA interfaces. The processor is a 4-core Intel, and 16 GB of RAM can easily handle multiple instances of NextCloud. Unlike the other boards, ZimaBlade was developed specifically for NAS rather than for multiple IoT purposes, like the Raspberry Pi. Thus, the ZimaBlade was suitable for my cloud blade solution.

## Board
My solution was the **ZimaBlade 7700 NAS Kit**, which incluses:
  - The board ZimaBlade 7700
  - 16 GB of RAM
  - 2 Bay HDD Rack
  - SATA Y Cable
  - The power adapter
  - Mini Display port to HDMI

<img src="https://github.com/user-attachments/assets/444716aa-8e6d-4b66-b7b2-b73ec9077c2a" alt="Zimablade 7700 Nas Kit" width="450" height="400">

Costs: ~200€ (including Tax and spedition)


# How to chose the HDD
Before to chose the HDD it is very important do decide how many HDD use.

## How to chose the correct RAID
The use of RAID configuration is very important to increase the reliability of the data. There are differet RAID configuration, but only tow have to be noted: RAID 1 and RAID 5.

### RAID 1
RAID 1 or mirroring, is a RAID configuration that provides a high level of data redundancy. Essentially, it creates an identical copy of all data on two or more disks. This means that if one disk fails, the data can be recovered from the other disk without any data loss.

<img src="https://github.com/user-attachments/assets/48c12526-186e-46c0-979b-514f06ede598" alt="RAID1" width="450" height="300">

PROs:
 - High reliability: Data redundancy ensures significant protection against data loss in case of a disk failure.
 - Fast recovery times: In the event of a failure, the system can be quickly restored using the spare disk.
 - Improved read performance: Read operations can be distributed across both disks, improving overall performance.

Cons:
- High cost: Requires the purchase of two or more disks of the same size, increasing the initial cost of the system.
- Reduced storage capacity: The effective storage capacity is limited to the capacity of the smallest disk in the RAID group, as only half of the total capacity is usable for data.
- Poor write efficiency: Each write is performed on both disks, which can negatively impact write performance, especially for intensive workloads.

It is possible to summarize in: in case of failure RAID 1 is easy duplicate data on a new HDD and in a fast way but the space is devide in two. 


### RAID 5

<img src="https://github.com/user-attachments/assets/7cbbda0a-4561-45d9-a851-91b6093957ed" alt="RAID5" width="450" height="300">




## Which HDD chose
Chossing the board was not very timing consuming, I just whatched some videos on youtube, and I foud my solution. Instead,the HDD choise was not easy, it required long time. 





## Hard Disk Drive

I bought tow Seagate IronWolf Pro, 4TB, Hard Disk SATA da 6GBit/s, HDD, CMR 3,5" 7.200 RPM, Cache da 128 MB

<img src="https://github.com/user-attachments/assets/a2df0e7b-d8cb-4781-9425-a5c941cf5025" alt="HDD" width="300" height="400">

Costs: ~200€ each HDD (including Tax and spedition)


# How to chose the Board
There are multiple board solutions for NAS and cloud, e.g., Raspberry Pi 4/5 or Orange Pi, and all of them are good alternatives to the ZimaBlade. I decided to buy the ZimaBlade because it exposes two SATA interfaces. The processor is a 4-core Intel, and 16 GB of RAM can easily handle multiple instances of NextCloud. Unlike the other boards, ZimaBlade was developed specifically for NAS rather than for multiple IoT purposes, like the Raspberry Pi. Thus, the ZimaBlade was suitable for my cloud blade solution.


# How to chose the HDD
why 2 and not 3?

Chossing the board was not very timing consuming, I just whatched some videos on youtube, and I foud my solution. Instead,the HDD choise was not easy, it required long time. 


