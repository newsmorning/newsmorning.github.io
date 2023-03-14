---
title: "Discover the Ultimate Backup Solution for Linux! Backintime KDE Edition Review inside!"
ShowToc: true 
date: "2023-05-02"
author: "Stephanie Coello"
---
*****
# Discover the Ultimate Backup Solution for Linux! Backintime KDE Edition Review Inside!

Are you tired of the stress and worry that comes with losing important files on your Linux system? If so, then you're in luck! Today we're here to introduce you to the ultimate backup solution for Linux - Backintime KDE Edition! 

## What is Backintime KDE Edition?

Backintime is a free, open-source backup software designed specifically for Linux-based operating systems. KDE Edition is a version of the software optimized for users of the KDE Plasma desktop environment. 

With Backintime KDE Edition, you can easily backup your entire Linux system, from your home directory to your system files. You can also automate your backups to run on a set schedule, ensuring that you never forget to backup your important files again. 

## Features of Backintime KDE Edition

There are several features that make Backintime KDE Edition the ultimate backup solution for Linux users. 

### 1. Simple Interface

Backintime KDE Edition has a simple, user-friendly interface that makes it easy for even novice Linux users to backup their important files. The interface is designed to be intuitive and easy to navigate, so you won't have to spend hours trying to figure out how to use it. 

### 2. Incremental Backups

One of the standout features of Backintime KDE Edition is its support for incremental backups. This means that the software will only backup files that have been added or changed since the last backup. This saves both time and storage space, ensuring that your backups are fast and efficient. 

### 3. Automated Backups

With Backintime KDE Edition, you can easily set up automated backups to run on a regular schedule. This means that you won't have to remember to backup your files manually - the software will do it for you. 

### 4. Version Control

Backintime KDE Edition also features version control, which allows you to keep multiple versions of your files. This is useful if you want to go back to a previous version of a file, or if you need to restore a file that has been accidentally deleted or overwritten. 

## How to Use Backintime KDE Edition

Using Backintime KDE Edition is incredibly simple. First, you'll need to install the software on your Linux system. You can do this by using your system's package manager, or by downloading the source code from the Backintime website. 

Once you've installed the software, you'll need to create a new backup profile. This profile will determine what files and directories are backed up, as well as how often the backups are run. 

When you're ready to run a backup, simply click the "Backup" button in the Backintime KDE Edition interface. The software will then create a new backup of your selected files and directories. 

## Conclusion 

If you're a Linux user looking for the ultimate backup solution, look no further than Backintime KDE Edition. With its simple interface, support for incremental backups, and automated backups, Backintime KDE Edition makes it easy to backup your important files and keep them safe from loss. Give it a try today and see just how easy it can be to keep your Linux system backed up and secure!

{{< youtube tXGVzMUsuE4 >}} 



Mac OS X users enjoy a slick Apple utility called Time Machine, while users of the latest Microsoft OS have Windows Backup. My install of Kubuntu Precise, oddly enough, didn’t come with a back-up utility installed out of the box. But, as always, we Linux users have a variety of options to choose from. Being the diehard KDE fan that I am, I looked for something that would fit in with my desktop, and settled on Backintime. Here’s a review.

 
## Installing & Launching
 
Like most applications in an Ubuntu-based system, installing this couldn’t be any easier:
 
For you “mainstream” Ubuntu fans, there’s also a GNOME-based version of this:
 
In another weird turn of events in my Precise system, the installation didn’t create an entry in the menu for this (it appeared under the “System” menu in Oneiric), but a quick command in KRunner did the trick:
 
## Usage
 
Once the application is launched, configuring it is reasonably straightforward. The main screen lists all the backup’s (Backintime calls them “Snapshots”) you’ve taken in the past (the column to the left in the figure below), a couple shortcuts (the top of the center column), a list of folders currently set to be backed up as a Snapshot, and a list of folders on your machine in the right column.
 

 
To configure your backups, click on the wrench icon in the main toolbar, which will display a configuration screen. Backintime has you create a “profile” that contains all the settings it needs. The dialog will have a profile (called “Main Profile”) already created when after you launch the app for the first time, but you can create different ones by using the “Add” button at the top of the dialog box (“Edit” and “Delete” should be self explanatory). The first tab of the dialog asks you to select where your Snapshots will be stored (I’m storing mine on an external hard drive), and at the bottom if you’d like to have backups scheduled to happen automatically… there are a couple different options.
 
The “Auto Host/User/Profile Id” checkbox is best left selected, as it will let Backintime handle the creation of some folders. What these fields mean is that my Snapshots will be stored in “/media/NETDOCK/backintime-rig/acp-rig/aaron/1”.
 
The next tab allows you to specify files and folders to be included in the Snapshot using the “Add File” and “Add Folder” buttons. I’ve included my entire home directory in the screenshot below. The third tab allows you to exclude folders in the same way. Backintime will fill this in with some reasonable defaults, so it doesn’t backup directories like Dropbox or Ubuntu One (which are already backed up in the cloud), temporary files, and backups of other backups (although you may still want these.
 
The fourth tab, “Auto-Remove,” lets you configure how many Snapshots you’d like to keep, and for how long you’d like to keep them. The “Options” and “Expert Options” let you set some minor configurations, like whether you’d like notifications when Backintime runs, but you’re safe leaving these as-is. Click “OK” to save your profile.
 
Once you’ve configured your profile, you can take your backup one of two ways:
 
- If you set the “Schedule” pull-down on the first (“General”) tab to “Disabled,” clicking the floppy disk button at the far left of the toolbar will start the snapshot for you.
 - If you set the “Schedule” pull-down to something else (like “Every day”), all you need to do is wait.

 
## Review
 
Backintime is a great example of how free software can be combined (in this case, Backintime is a combination of software including rsync, cron, the backintime core files, and a KDE interface) to create something more user-friendly than the pieces on their own. Certainly, a casual (or even intermediate user) will have a much easier time configuring backups for his/her system than with something like rsync alone.
 
That said, the interface is a little cluttered and confusing. The lists of folders on the main screen make me assume you can use them to configure a backup, e.g. via drag-and-drop, but this isn’t the case. The list of folders on the right of the main screen might appear to be simply there for reference (with an option to copy the current path, presumably to paste it into one of the tabs in the config screen), but they’re also there so you can view the differences/changes between Snapshots at the folder level. The Restore button is tucked in among four buttons, none of which are particularly well labelled. As a result, it’s probably easy for most users to configure the backup, but restoring all or part of those backups will be more frustrating.
 
However, it’s ability to take scheduled backups with no interaction from the user make Backintime a perfectly usable, if not completely intuitive, solution to make sure all the files on your Linux box are safe.
 
Image credit: Backup, written in red ink. by Big Stock Photo.
 
Aaron is an interactive business analyst, information architect, and project manager who has been using Linux since the days of Caldera.  A KDE and Android fanboy, he'll sit down and install anything at any time, just to see if he can make it work.  He has a special interest in integration of Linux desktops with other systems, such as Android, small business applications and webapps, and even paper.
 
Our latest tutorials delivered straight to your inbox



