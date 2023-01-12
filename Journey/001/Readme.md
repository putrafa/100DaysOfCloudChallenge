# Virtualisasi and Basic Linux 
## Introduction

As a beginner in the cloud field, I have to learn and understand the basics first, namely virtualization and basic Linux.
1. Meet 1 (Mentors : Diana Zuniarti)
2. Virtualization introduction
3. Linux Fundamental
4. Hirarki File Linux
5. Basic Command Linux
## Cloud Research

The first day I attended a meet on Zoom apk which was mentored by Diana Zuniarti and learned about virtualization and basic Linux.
1. Virtualization Introduction
  - Definition
    A virtual machine is a software program or virtual operating system that can run on a piece of hardware along with the device's native OS. A virtual machine is a virtual server environment that works like a computer within a computer. The virtual machine runs on an isolated partition on the host computer with its own resources such as CPU, memory, and operating system. This allows the user to run various applications on the virtual machine and use them as they normally would on that device.
  - Functions and Benefits
    - Easily switch between multiple operating systems on a single physical device
    - Can be used to perform tests on different operating systems
    - Testing software on many different OS is also easier, you don't have to have multiple devices to do it
    - Used for compiling several different servers on one device
![Screenshot](https://user-images.githubusercontent.com/121589476/211958791-88358c13-161d-4ec0-a2dc-be72d98796d0.png)
Image Source: Youtube Aguna Course - Introduction to Virtual Machines

2. Linux Fundamental
   Linux is a Unix-based operating system, in other words, Linux is a derivative of Unix. Linux is an operating system that is multi-user and multi-tasking. This means that more than one user can execute more than one process (program) at the same time. Linux is a free computer operating system created by a community of open source developers. Linux serves as an alternative to Windows or the more popular OS/X. In simple terms, Linux is an operating system or Operating System (OS), just like Windows OS, MacOS, iOS, Android, and so on. Like any other operating system, Linux's function is as a container for bridging communication or user commands on the relationship between software and hardware in a device.

3. Hirarki File Linux
   The root directory, represented by “/”, is the top level directory on the system. It contains files and subdirectories that are essential for system functioning.
   Structures and Directories in Linux :
   - Structures :
  
![Screenshot](https://user-images.githubusercontent.com/121589476/211962825-e299cecc-1ec9-405d-9d3f-b83bd0d5c7db.png)
- /root : the highest directory, above the root system directory
- /bin : contains executable files for use by the system
- /boot : contains files for booting the operating system
- /dev : contains device files
- /etc : where to store the configuration
- /home : to store the user's files
- /media : mount point for mobile storage media such as CD-ROM, USB, Floppy and others
- /lib : contains library files
- /mnt : used to mount temporary files
- /proc : contains files that have information about the processes being run by the operating system
- /sbin : the same as /bin, only binary files are stored
- /opt : a directory that is rarely used on Linux and is usually used for third party software and not utilities from the GNU Project such as java applications or virtualbox
- /tmp : contains temporary files that are used while the operating system is running
- /usr : this directory can be used by all users for various purposes, such as sharing folders
- /var : contains variable files, such as mail, log files

4. Basic Commands on Linux :
- cd : command to enter the desired directory
- cp : command to copy files/directories
- mv : command to move files and can also rename files
- touch : command to create a file
- rm : command to delete files
- mkdir : command to create directories
- cp -r : command to copy the directory and its contents
- rmdir : command to remove empty directories
- clear : command to clear the display on the screen
- history: command to see what commands we have run
- nano : command to edit files
- ls : view the contents of the directory
- pwd : to show our current position
- echo "..." : to add a sentence to the file
- echo "..." : to replace the contents of the file and be replaced with the sentence in the command
