---
title: "Protect Your Sensitive Data Forever: Discover the One Command You Need to Lock Up Files and Stop Unauthorized Changes!"
ShowToc: true 
date: "2023-07-05"
author: "Brian Heath"
---
*****
Protect Your Sensitive Data Forever: Discover the One Command You Need to Lock Up Files and Stop Unauthorized Changes!

In an increasingly connected world, protecting your sensitive data has become more important than ever before. Hackers and cyber criminals are constantly on the lookout for vulnerabilities in computer systems, and a breach of your data can have serious consequences. From identity theft to financial loss, the risks are high.

But how can you protect your sensitive data? One simple command on your computer can help you lock up files and stop unauthorized changes. In this article, we will explain what the command is and how to use it.

The command in question is called chmod. Chmod is a command used in Unix-based operating systems, including Linux and macOS. It stands for "change mode" and is used to change the permissions of files and directories.

To use chmod, you first need to open a terminal window. In a Linux computer, you can do this by pressing Ctrl+Alt+T. In a macOS computer, you can do this by pressing Command+Space and typing "Terminal" in the search bar. Once you have the terminal window open, you can proceed with the following steps:

Step 1: Identify the file or directory you want to protect

Before you can use chmod, you need to identify the file or directory you want to protect. To do this, navigate to the folder where the file or directory is located using the cd command. For example, if you want to protect a file called "mydata.txt" located in the Documents folder, you can type:

cd /Users/yourusername/Documents

This will take you to the Documents folder.

Step 2: Check the current permissions of the file or directory

Once you are in the folder where the file or directory is located, you can check the current permissions using the ls -l command. This will show you a list of files and directories in the current folder, along with their permissions. For example, if you want to check the permissions of "mydata.txt", you can type:

ls -l mydata.txt

This will show you the permissions of the file, which will look something like this:

-rw-r--r-- 1 yourusername yourgroup 1256 Oct 20 13:45 mydata.txt

The first column (starting with "-") shows the file type and permissions. The next two columns show the owner (yourusername) and the group (yourgroup). The last column shows the file name.

Step 3: Change the permissions of the file or directory

Now that you know the current permissions of the file or directory, you can use chmod to change them. There are three types of permissions you can change: read, write, and execute. Each permission can be set for the owner, the group, and others. The permissions are represented by numbers:

4 - read
2 - write
1 - execute

To set the permissions, you need to add up the numbers for each type of permission. For example, to give the owner and group read and write permissions, and others no permissions, you can type:

chmod 660 mydata.txt

The first "6" represents read and write permissions for the owner. The second "6" represents read and write permissions for the group. The "0" represents no permissions for others.

Step 4: Verify the new permissions

Once you have changed the permissions using chmod, you can verify that they have been set correctly using the ls -l command again. For example, if you want to verify the permissions of "mydata.txt", you can type:

ls -l mydata.txt

This should show the new permissions you set earlier.

Conclusion

With just one command, you can protect your sensitive data from unauthorized changes. Chmod is a simple yet powerful command that can help safeguard your files and directories. By using it correctly, you can ensure that your data is secure and protected forever.

{{< youtube YiVkbOggOBQ >}} 



To unlock:
 
Explanation: chattr is a command that allows a user to set certain attributes on a file residing on a Linux filesystem. A “+i” flag adds an immutable attribute to the file. When this is enabled, even a root user cannot change the file. Similarly, a “-i” flag subtracts the specific attribute from the file.
 

 
If you have a folder of files that you want to lock up, you can also add the “+R” flag. For example:
 
Note: Only the superuser or a process pessessing the CAP_LINUX_IMMUTABLE capability can set or clear this attribute. 
 
Damien Oh started writing tech articles since 2007 and has over 10 years of experience in the tech industry. He is proficient in Windows, Linux, Mac, Android and iOS, and worked as a part time WordPress Developer. He is currently the owner and Editor-in-Chief of Make Tech Easier.
 
Our latest tutorials delivered straight to your inbox



