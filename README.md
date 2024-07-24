# My Journey in Cloud self-hosting

### Table Of Contents
- Introduction
- Hardware
- File-system
- Cloud configuration

## Introduction
Creating a personal cloud is a long journey. It requires a lot of time to investigate which solution is best for you at the moment of creation. I explored multiple technologies, both hardware and software, to create my homemade cloud device based on my requirements. I decided to post my journey to help those who want to explore cloud self-hosting. Basically, this post is a guide for a younger version of myself looking for their solution. If I had had this post available, I would have had an easier path. Anyway, this journey has been very helpful for improving my skills and gaining an overview of a world that is not mine.

### Rationale
What I'm looking to create is a family cloud, where we can store photos or data with high reliability and integrity, for 4 or 5 people. The data must be reachable anywhere with a good user experience. Web applications and mobile applications for both Android and iOS must be available.
A very important point is security. Nobody must be able to access the system; even the system administrator (me) must not be able to access other people's data.
Moreover, price, the device must be "cheap" and must cousume less power as possible. 

### Consideration
This blog is not about how to create a self-hostesd cloud, is about how my cosideration my experience aboud self hotest, which could help you to take the best solution for you enviroment. My choeses could not match your wish. From this experiments I learned multiple new technologies which is not common to use in my daly routene. So, I could makes mistekes, I'm not a cloud developer, even a developer.

### About me
I'm self-hosting appassionate with a strong backgound in cybersecurity. I have more than 10 yeas os experience in cybersecurity, I tested from cybersecurity prospective multiple applications, from hardware to cloud bases. 

## Abstract
An home cloud can provide the privacy and the configuration tha no other online solution can provide. After a long jorney I decide to use a single board computer, with two HDD of 4TB each in mirroring. The Cloud software is based on NextCloud and the NAS capability is handled using ZFS file system.
