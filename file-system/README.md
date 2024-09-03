# File-system
Choosing the correct file system is essential for ensuring data reliability and efficiency. 
My solution involves adopting Open Zettabyte File System (ZFS). ZFS is designed to guarantee high data reliability by detecting data corruption and restoring it quickly and easily.

# TOC
 - EXT4 vs XFS vs BtrFS vs ZFS
 - How to configure ZTF in mirroring


# EXT4 vs XFS vs BtrFS vs ZFS
GNU/Linux is able to manage multiple file-system types. The most famous and used are EXT4, XFS, BtrFS and Open ZFS.

- **EXT4**, or Fourth Extended File System, is a widely-used file system in Linux environments, known for its reliability and performance. Key features of EXT4 include journal checksumming for improved data integrity, delayed allocation to boost performance, and extents, which improve the handling of large files and reduce fragmentation.
- **XFS** is a high-performance, journaling file system originally developed by Silicon Graphics and now widely used in Linux environments.
  Designed for scalability and efficiency, XFS excels in handling large files and high-capacity storage systems.
  Its key features include support for large file sizes and volumes, efficient space management, and advanced data integrity through journaling.
- **Btrfs**, or B-Tree File System, is a modern file system for Linux designed with advanced features and scalability in mind.
  Developed as a replacement for older file systems like EXT4, Btrfs offers robust data management capabilities, including support for snapshots, built-in RAID functionality, and dynamic volume resizing.
- **ZFS** (Zettabyte File System) is an advanced file system and volume manager originally developed by Sun Microsystems for the Solaris operating system, and now available for other platforms like Linux and FreeBSD. It is renowned for its robustness and scalability, integrating both file system and volume management into a single unified solution. ZFS ensures data integrity through its use of checksumming for both data and metadata, which helps detect and correct data corruption. It also incorporates self-healing capabilities, automatically repairing corrupted data using redundant copies, and includes built-in support for advanced RAID configurations. This combination of features makes ZFS a powerful and flexible choice for managing high-performance storage needs.

<div align="center">
 
|       Feature          |  EXT4  |   XFS   | Btrfs  |  ZFS  |
|:----------------------:|:------:|:-------:|:------:|:-----:|
| Expansion              |   ✅   |   ✅    |   ✅   |  ✅   |
| Reduction              |   ✅   |   ✅    |   ✅   |  ❌   |
| Logical volume manager |   ❌   |   ❌    |   ✅   |  ✅   |
| Checksum on data       |   ❌   |   ❌    |   ✅   |  ✅   |
| Checksum on metadata   |   ✅   |   ✅    |   ✅   |  ✅   |
| Compression support    |   ❌   |   ❌    |   ✅   |  ✅   |
| Filesystem encryption  |   ❌   |   ❌    |   ❌   |  ✅   |
| Copy on Write          |   ❌   |   ✅    |   ✅   |  ✅   |
| Snapshots              |   ❌   |   ✅    |   ✅   |  ✅   |

</div>

**Some consideration**: There are multiple other comparison features that should be noted, but the ones listed above, in my opinion, are the most important.

# How to configure ZTF in mirroring


