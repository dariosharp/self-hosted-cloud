# Hardware
My solution is composed by a single board computer and two Hard Disk Drive. I was looking for a low power consume computer and a reliable solution for the data. 
So the two hardware elements to chose are: 
 - The board (the computer), aim to manage all the software.
 - The disks, aim to manage all the data.

# TOC
 - Board
   - My Board Solution
 - Disks
   - How to chose the correct RAID
   - How to chose the Disks
   - My disks solution

# Board
There are multiple board solutions for NAS and cloud, e.g., Raspberry Pi 4/5 or Orange Pi, and all of them are good alternatives to the ZimaBlade. I decided to buy the ZimaBlade because it exposes two SATA interfaces. The processor is a 4-core Intel, and 16 GB of RAM can easily handle multiple instances of NextCloud. Unlike the other boards, ZimaBlade was developed specifically for NAS rather than for multiple IoT purposes, like the Raspberry Pi. Thus, the ZimaBlade was suitable for my cloud blade solution.

## My Board solution
My solution was the **ZimaBlade 7700 NAS Kit**, which incluses:
  - The board ZimaBlade 7700
  - 16 GB of RAM
  - 2 Bay HDD Rack
  - SATA Y Cable
  - The power adapter
  - Mini Display port to HDMI

<img src="https://github.com/user-attachments/assets/444716aa-8e6d-4b66-b7b2-b73ec9077c2a" alt="Zimablade 7700 Nas Kit" width="450" height="400">

Costs: ~200€ (including Tax and spedition)


# Disks
Chossing the board was not very timing consuming, I just whatched some videos on youtube, and I foud my solution. Instead,the HDD choise was not easy, it required long time. There are multiple thing to take in mind. Before to chose the disk it is very important do decide how many HDD use, so the RIDE type to use.

## How to chose the correct RAID
The use of RAID configuration is very important to increase the reliability of the data. There are differet RAID configuration, but only two have to be noted: RAID 1 and RAID 5.
For more details: https://en.wikipedia.org/wiki/RAID

I decided to use RAID 1 because is easier and faster to replace a failure disk. 


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

**Overall**: in case of failure on a disk, RAID 1 is easy duplicate data on a new HDD and in a fast way but the space is devide in two. 


### RAID 5
RAID 5 is a popular storage configuration that offers a balance between performance, redundancy, and cost-effectiveness. However, it's essential to understand its strengths and weaknesses before implementing it.

<img src="https://github.com/user-attachments/assets/7cbbda0a-4561-45d9-a851-91b6093957ed" alt="RAID5" width="450" height="300">

Pros of RAID 5:
  - Data redundancy: Protects against the failure of a single drive.
  - Improved read performance: Can significantly boost read speeds compared to a single drive.
  - Cost-effective: Generally more affordable than other RAID levels offering similar redundancy.
  - Good balance of performance and redundancy: Provides a reasonable compromise between speed and data protection.

Cons of RAID 5:
  - Write performance penalty: Due to parity calculations, write speeds can be slower compared to other RAID levels.
  - Single point of failure: If two drives fail simultaneously, data loss is likely.
  - Rebuild time: Rebuilding a failed drive can be time-consuming and resource-intensive.
  - Reduced usable capacity: One drive's worth of storage is used for parity information.
    
**Overall**: in case of failure on a disk, RAID 5 require a lot of time to duplicate data on a new HDD but the space is devide in 1/3.


## How to chose the disks
Once decided the RAID it time to decide what type HDD buy. Even if HDD appear an easy task to chose, it is important to be carefoul and take in in mind a couple of thinks. 
- Fists the space: more TBs the HDD has more likely are failures. So it is generally not reccomanded to buy.
- Second the tecnology: SSD or HDD? SSD is more expensive then HDD but reuire less energy and more reliable. I decide use HDD due to the price, SSD today is 2.5 time the price of HDD.
- Third CMR vs SMR: 
  - CMR (Conventional Magnetic Recording)
    - Pros: Faster read and write speeds, especially for random data access.
    - Cons: Lower storage density compared to SMR.

  - SMR (Shingled Magnetic Recording)
    - Pros: Higher storage capacity for the same physical size.
    - Cons: Slower write speeds, especially when overwriting existing data.
    
- Last but not leas: It is reccomended to do not buy the HDDs or SSD from the same reseller at the same time. Buying the same disks at same reseller, could increase the chanse to have the same failure at the same time becouse the disk can be came from the same block of creation. So consider to buy the disk from two different reseller. 
    
  Overall: HDDs CMR bought from different reseller garantee high standard reialability and a not expensive solution. 

## My disks solution

I bought tow Seagate IronWolf Pro, 4TB, Hard Disk SATA da 6GBit/s, HDD, CMR 3,5" 7.200 RPM, Cache da 128 MB

<img src="https://github.com/user-attachments/assets/a2df0e7b-d8cb-4781-9425-a5c941cf5025" alt="HDD" width="300" height="400">

Costs: ~200€ for both the HDDs, ~100€ each on amazon (including Tax and spedition)



