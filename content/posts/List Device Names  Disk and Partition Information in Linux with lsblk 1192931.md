---
title: "Discover the Secret Linux Trick to Uncover Device Names and Partition Details with One Simple Command!"
ShowToc: true 
date: "2023-02-04"
author: "James Garner"
---
*****
Introduction

Linux is a robust and powerful operating system that offers a wide range of functionalities to its users. However, working with the Linux command-line interface (CLI) can be quite challenging, especially for new users. One of the common challenges that users face is identifying device names and partition details. Luckily, Linux offers a simple command that can unveil this information in one shot. In this article, we’ll explore the secret Linux trick that can help you uncover device names and partition details with one simple command!

What is the Secret Linux Trick?

The secret Linux trick that we’re referring to is the "lsblk" command. The lsblk command stands for "list block devices," and it is used to display information about all available block devices (e.g., hard drives, SSDs, USB drives, etc.) and their respective partitions. When you run the lsblk command, Linux will output a tree-like hierarchy of your block devices and their partitions. The output will include the device name, partition name, MountPoint, file system type, and the size of each partition.

How to Use the lsblk Command

Using the lsblk command is straightforward. Open your terminal and type the following command:

$ lsblk 

After pressing enter, Linux will output a tree-like hierarchy of all the available block devices and their partitions. The output will look something like this:

NAME    MAJ:MIN RM   SIZE RO TYPE MOUNTPOINT
sda       8:0    0 238.5G  0 disk
├─sda1    8:1    0  100M  0 part /boot/efi
├─sda2    8:2    0  512M  0 part /boot
├─sda3    8:3    0  100G  0 part /
└─sda4    8:4    0 138.9G  0 part /home

From the output above, you can tell that there's a block device named "sda" with four partitions (sda1, sda2, sda3, and sda4). Each partition has its size, file system type, and MountPoint. In this case, sda3 is the root partition, and sda4 is the home partition.

Additional Options

The lsblk command also offers other output options that can enhance the information provided by the command. For instance, you can display the output in a more readable format using the "-f" option. Here's how:

$ lsblk -f

The "-f" option will display the output in a more user-friendly format that includes the file system type of each partition.

NAME    FSTYPE   LABEL       UUID                                 MOUNTPOINT
sda             
├─sda1 vfat                 4D21-8E4E                            /boot/efi
├─sda2 ext4                 bddeee70-96f2-4c0b-9cdd-9b472485ad4a   /boot
├─sda3 ext4                 d96f0255-5ae9-4e5f-b3e3-842c77a8f1d3   /
└─sda4 ext4     myhome      e2f219a7-25cb-4b60-8d38-65bf36f7b53e   /home

Similarly, the lsblk command allows you to specify a specific device or partition to display information about. For example, to display information about the sda3 partition, you can run the following command:

$ lsblk /dev/sda3

Conclusion

In conclusion, the lsblk command is a powerful utility that can unveil critical information about your Linux block devices and their partitions. By running the lsblk command, you can easily identify device names, partition details, MountPoints, and file system types. This information is crucial, especially when mounting external storage devices, creating new partitions, or troubleshooting disk-related issues. So, the next time you’re working with Linux, don’t forget to use the secret lsblk command to uncover device names and partition details with one simple command!

{{< youtube Mv0VhAgbL8o >}} 



On Linux, you sometimes need to work with disks and/or partitions directly from the command line. Often, you actually want to perform actions on the filesystems, but you do so by specifying the partitions where they are stored. On the command line, you refer to these by using their device names (for example, “/dev/sda3”).
 
On systems with many disks, partitions, optical drives, and USB drives, it can be hard to identify the device name assigned to each of them.
 
## What Does the lsblk Command Do?
 
lsblk displays information about storage devices. The utility is most often used to identify the correct device name to be passed to a subsequent command.
 

 
Most of the time, lsblk without any additional parameter, suffices to help identify the disk or partition you want to work with. From the picture above, for example, I can tell that “sda4” is a Windows partition, but that’s because I know its size is approximately 200GB. However, if you have two or more partitions of the same size, things may get more confusing. In other cases you may simply not know or remember the size of a particular disk or partition on your system.
 
On Linux, it’s dangerous to confuse device names, as you may destroy or corrupt useful data with a wrong command.
 
## Useful lsblk Parameters
 
By default, lsblk displays just a few properties, as you saw in the picture above. But, if you add parameters to the command, you can make it output additional device properties. This, in turn, makes it much easier to identify the disk or partition you are looking for.
 
### Find Out If It’s an SSD or Hard-Disk (HDD)
 
To see what extra columns lsblk can display, enter the following:
 
In this scenario you will use ROTA and DISC-GRAN. ROTA tells you if a block device belongs to a rotational storage device. Hard disks are rotational, so the column outputs “1” besides them (binary logical value meaning “true”). DISC-GRAN shows you the discard granularity. SSDs support discard to free up unused data blocks. Hard disks do not support this feature, since they don’t need it, so this column will display a zero value for them (“0B,” meaning discard granularity of zero bytes).
 
### Show Filesystems Stored on Disks/Partitions
 
When you see a list of partitions, you might be able to tell what each of them stores, based on their sizes alone. When this is not enough, you can make lsblk output filesystems, too. It’s much easier to identify partitions this way because:
 
- Windows uses the NTFS filesystem
 - Linux usually uses ext4
 - A USB device uses FAT, FAT32 (vfat) or NTFS
 - The EFI boot partition is usually very small and shows a vfat filesystem on it

 
Also, add the LABEL output column, which can help if partitions have been labeled when created/formatted.
 
### Show Removable Devices/USB Memory Sticks
 
will display an extra column that tells you if the device is removable. A “1” value means “true,” which indicates a USB stick or other types of removable media.
 
### Show HDD/SSD Model
 
This is useful when you want to look up the exact code of your storage device model to upgrade your firmware or download drivers.
 
### Show Filesystem UUID (Universally Unique Identifier)
 
Older Linux distributions mounted filesystems by specifying their device names in “/etc/fstab.” However, that proved unreliable since “/dev/sda2” might become “/dev/sdb2” when you add another storage device to the system. Nowadays, UUIDs are used instead, which remain constant no matter what you add/remove to/from your computer. For whatever reason you need UUIDs, you can make lsblk display them with
 
## Show Other lsblk Columns You Need
 
At the beginning of the tutorial, you used
 
to see extra columns that lsblk can display. If the examples here are not sufficient for your needs, consult that help information again and combine parameters as needed. To do so, just enter lsblk -o +, followed by the column names that you want to output. Separate column names with a comma (“,”). For example:
 
## Conclusion
 
After you identify the device name you want to work with, remember to replace it with the full device path in the subsequent command you intend to use. For example, if you got “sda4” as a result in lsblk, you will have to replace it with “/dev/sda4” in the next command. So, instead of “sda4” you type “/dev/sda4” in a command like mkfs -t ext4 /dev/sda4.
 
Fell in love with computers when he was four years old. 27 years later, the passion is still burning, fueling constant learning. Spends most of his time in terminal windows and SSH sessions, managing Linux desktops and servers.
 
Our latest tutorials delivered straight to your inbox



