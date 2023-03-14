---
title: "Unveiling the Secret Linux Boot Process! Learn What You Should Know to Master Your System"
ShowToc: true 
date: "2023-03-26"
author: "Elizabeth Oconnell"
---
*****
### Unveiling the Secret Linux Boot Process!

#### Learn What You Should Know to Master Your System

As a Linux user, it is essential to understand the boot process thoroughly. The boot process refers to the sequence of events that the system undergoes when it is switched on, leading to the point where it is fully functional.

The boot process is divided into several stages, and by understanding each step, you can troubleshoot problems and optimize your system's performance.

Here is a detailed outline of the boot process in Linux:

1. BIOS/UEFI: This is the first stage of the boot process. When the system is powered on, the BIOS/UEFI firmware performs a Power-On Self-Test (POST) to check the hardware components such as the CPU, RAM, and hard drives. The firmware then reads the boot loader from the primary boot device and loads it into memory.

2. Boot Loader: The job of the bootloader is to load the operating system into memory. There are several bootloaders available for Linux, but the most common one is GRUB (Grand Unified Bootloader). GRUB reads the configuration file (/boot/grub/grub.cfg) and loads the Linux kernel.

3. Kernel: The Linux kernel is the core of the operating system, and it controls all the system's hardware and software components. The kernel loads drivers for the various hardware components and starts the init process.

4. Init Process: The init process is the first user-space process that is started by the kernel. It is responsible for starting system services, such as networking, disk management, and user login. In most Linux distributions, the init process has been replaced by systemd.

5. Systemd: Systemd is the new init system that has replaced the traditional SysV init system. Systemd is responsible for managing system services, and it also takes care of system initialization and shutdown.

6. Login Manager: The Login Manager is the graphical user interface that prompts the user to log in. The Login Manager starts the user's desktop environment after the user has entered their credentials.

7. Desktop Environment: The Desktop Environment is the graphical user interface that the user interacts with. It is responsible for managing windows, applications, and other user interface elements.

By understanding the boot process in Linux, you can optimize your system's performance, troubleshoot problems, and even create custom boot configurations.

For example, you can modify the GRUB configuration file to remove unnecessary boot options, enabling your system to boot faster. You can also add custom scripts to the init process to load system services in a particular order, ensuring that critical services are loaded first.

In conclusion, the boot process in Linux is complex, but by understanding each stage of the process, you can control your system's behavior and optimize its performance. Take the time to study the boot process, and you will be well on your way to mastering your Linux system.

{{< youtube AOHI9U8phDw >}} 



Ever been curious about the different stages of Linux, an open-source operating system? Knowing the entire boot process can help you troubleshoot issues – especially if you’re the administrator.
 
What happens behind the scenes when you power your device on? Read on to find out.
 
## BIOS
 
The Basic Input/Output System (BIOS) is a piece of low-level firmware stored on a small memory chip in your computer’s motherboard. This firmware aids the start-up process and manages data flow between your machine and other connected devices, such as a mouse, printer and video adapter.
 

 
The primary function of BIOS, shown above, is to run the Power-On Self Test (POST). This test verifies the operability of system hardware and finds the boot sector, which contains the software necessary for the rest of the process. If the POST is successful, the BIOS will load the next step, the Stage One Boot Loader, into the system’s RAM.
 
If the POST isn’t successful, the BIOS will return a code you can use for troubleshooting.
 
## Stage One Boot Loader
 
The first stage of the boot loader — called the Master Boot Record (MBR) or Guided Partition Table (GPT) — is designed to get the program online.
 
The MBR is a simple piece of software with no built-in understanding of file systems. As a result, you will always need to store the stage two boot loader between the MBR and the first partition on the hard drive.
 
Once the MBR detects the stage two boot loader, it hands over control.
 
## Stage Two Boot Loader
 
The job of the stage two boot loader is to find the kernel and load it into memory.
 
Most Linux divisions will use one of three different boot loaders — GRUB, GRUB2 or LIL. You’ll most likely see GRUB2, depicted below, as it’s the newest.
 
Once the boot loader has found a kernel and loaded it into RAM, it passes over control. It also sends an image of your device’s file system the kernel can use to find modules.
 
## Kernel
 
Because all kernels exist in a compressed format to save hard drive space, the first thing it will do once given control is self extract. Then it will mount the image version of the file system it received from the boot loader.
 
The kernel will detect the system’s hardware and swap over the image to the root file on disk.
 
## init (systemd)
 
Next, the kernel will start the initialization (init) system – the first process which spawns all processes necessary for the booting process. On most systems, this will be systemd.
 
Systemd’s primary function is to launch all of the daemons – background processes and services – needed to run the system. These services will continue to run after initialization and manage essential system processes like logging various system messages, keeping track of devices and ensuring that the file system is synchronized with system memory.
 
If you’re curious about which services systemd is running, running the systemctl command by itself will return a full list.
 
You can also use systemd to start other services on boot by using a combination of the systemctl command and the service you want to start. For example, if you want the system to check the status of the NFS, you can type systemctl status nfs-server.service. You can also start, stop, enable or disable a service with a combination of systemctl and one of those commands.
 
## Runlevel
 
The run level is a state of INIT, and your system defines what services are running. The standard Linux kernel supports seven different runlevels:
 
- 0: System halt, ready to be powered off
 - 1: Single user mode
 - 2: Multiple user mode, no network file system
 - 3: Multiple user mode using the command life interface instead of the graphical user one
 - 4: User-defined
 - 5: Multiple user mode, using the graphic user interface that most Linux systems will boot into by default
 - 6: Reboot

 
If you need to change the runlevel for any reason, INIT will be responsible for altering it using the telinit command, shown above.
 
## Breaking Down the Boot Process
 
This breakdown is merely an overview of the Linux boot process and leaves out some of the finer details. However, it should give you the information you need to troubleshoot any problems you may face.
 
Our latest tutorials delivered straight to your inbox



