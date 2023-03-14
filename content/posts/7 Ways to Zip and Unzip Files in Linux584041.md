---
title: "Unleash The Power Of Linux: 7 Mind-Blowing Ways To Zip and Unzip Files!"
ShowToc: true 
date: "2022-12-03"
author: "Donna Sheppard"
---
*****
Title: Unleash The Power Of Linux: 7 Mind-Blowing Ways To Zip and Unzip Files!

Subtitle: Discover The Top Tricks and Techniques To Zip and Unzip Files With Ease On Linux

Introduction:

Linux is an incredibly versatile operating system that offers unparalleled flexibility, security and stability. One of the many benefits of using Linux is that it makes it remarkably simple to zip and unzip files, a process that is both essential for managing large archives, and also handy for reducing file sizes to save space or speed up transfers.

In this article, we will take an in-depth look at the top 7 mind-blowing ways to zip and unzip files on Linux. These powerful techniques and tricks will help you process files more efficiently, offer greater customization and control, and ultimately make the most of the power and capability of Linux.

1. The Command Line:

The simplest and most powerful way to zip and unzip files on Linux is by using the command line. With the command line, you have absolute control over the zipping and unzipping process, and can perform complex operations with ease.

To zip a file using the command line, run the following command:

$ zip archive.zip file1.txt file2.txt

This command will create a new archive file called "archive.zip" and add the files "file1.txt" and "file2.txt" to it. To unzip an archive file, run this command:

$ unzip archive.zip

This command will extract all the files contained in the archive to the current directory.

2. 7-Zip:

7-Zip is a popular file archiver that can be used on Linux. It supports a wide variety of formats, including ZIP, RAR and 7z. To install 7-Zip on Ubuntu, run the following command:

$ sudo apt-get install p7zip

To create a new archive with 7-Zip, use the following command:

$ 7z a archive.7z file1.txt file2.txt

To extract files from an archive, use this command:

$ 7z x archive.7z

3. TAR:

TAR is an older format that is still widely used on Linux. It is often used in conjunction with GZIP or BZIP2 to create compressed archives. To create a TAR archive with GZIP compression, run the following command:

$ tar -czvf archive.tar.gz file1.txt file2.txt

To extract files from a TAR archive, use this command:

$ tar -xzvf archive.tar.gz

4. RAR:

RAR is a popular archive format that is widely used in Windows. However, there is a Linux version of RAR that can be used to create and extract RAR archives on Linux. To install RAR on Ubuntu, run the following command:

$ sudo apt-get install unrar

To create a new RAR archive, use the following command:

$ rar a archive.rar file1.txt file2.txt

To extract files from a RAR archive, use this command:

$ unrar x archive.rar

5. Zip and Unzip GUI Tools:

Linux also offers a number of graphical user interface (GUI) tools for zipping and unzipping files. The most popular of these tools is Archive Manager, which is included in most Linux distributions. Archive Manager provides a simple and intuitive interface for creating and extracting archives.

To create a new archive with Archive Manager, simply right-click on the files you want to add to the archive, and select "Compress". To extract files from an archive, double-click on the archive file and select "Extract".

6. PeaZip:

PeaZip is a free, open-source file archiver that supports a wide variety of formats, including ZIP, RAR and 7z. It is available for Linux, Windows and macOS. To install PeaZip on Ubuntu, run the following command:

$ sudo apt-get install peazip

To create a new archive with PeaZip, use the following command:

$ peazip archive.zip file1.txt file2.txt

To extract files from an archive, use this command:

$ peazip -ext archive.zip

7. Ark:

Ark is another popular file archiver for Linux. It supports a wide variety of formats, including ZIP, RAR and TAR. It is included in most Linux distributions.

To create a new archive with Ark, simply right-click on the files you want to add to the archive, and select "Create Archive". To extract files from an archive, double-click on the archive file and select "Extract".

Conclusion:

Linux offers a wide variety of powerful and flexible tools for zipping and unzipping files. Whether you prefer using the command line or a GUI tool, there is something for everyone. The top 7 mind-blowing ways to zip and unzip files on Linux that we have discussed in this article are just the beginning. With Linux, the possibilities are endless! So, get started today and unleash the power of Linux!

{{< youtube F1GshnAYrII >}} 



More and faster are always two things we want, especially when it comes to data. The problem is that “more” and “faster” are usually at odds, so we have file compression. There are several ways to zip and unzip files in Linux, and we’re going to show you the methods behind them.
 
## Zip and Unzip Using Zip in Linux
 
Linux has several compression tools built into almost every distribution, commonly known as Linux distros. Zip is likely the most popular. The Zip utility can be used in the graphical user interface (GUI) or the terminal.
 
## Zip in the Linux GUI
 
- Navigate to the files to be compressed and select them. Then right-click and select Compress.

 
- Enter a name for the zipped archive. Note that you can also choose two other types of compression. This may vary between distros.

 
- Soon you’ll see your zipped archive. Note that the archive size is much less than the total size of the files put into it.

 
## Unzip in the Linux GUI
 
- Find the zipped archive to unzip and right-click on it. Select Extract Here or Extract to…. Extra Here puts the contents into this directory. Extract to… allows you to select somewhere else to put the contents.

 
The files are extracted. Notice that they’re back to their full size of 100 MB each.
 

 
## Archive Manager to Unzip in the Linux GUI
 
Some Linux distros have other ways to unzip built into them. In this example, you can use Archive Manager.
 
- Right-click on the archive and select Open With Archive Manager.

 
- Highlight the files to extract by single-clicking on them. You can select one, a few, or all of them. Then select Extract in the top-left corner.

 
- At this point, you can choose where to extract the files using the file manager. Then select Extract in the top-right corner.

 
- When the extraction is done, you can either carry on or Show the Files.

 
The file is back at its full size. A copy is left inside the archive.
 
## Zip Files in Linux Terminal
 
Open the terminal and navigate to the directory where the files to be zipped are located. Enter the command zip ziptest.zip *. 
 
Zip tells Linux to use the zip utility, ziptest.zip tells it the desired name for the archive, the asterisk (*) is a wildcard meaning zip all the files in this directory. 
 
It zips the files, lists them, and says how much it has deflated or compressed them.
 
Many actions can be used with the zip command. To view them, enter zip –help, and you’ll see something like the following image.
 
## Unzip Files in Linux Terminal
 
In the Terminal, use the command unzip ziptest.zip, where unzip is the command and ziptest.zip is the name of the archive to unzip.
 
It will show the files being unzipped, so you know when it’s done.
 
Like the zip command, many actions can be used with the unzip command. To view them, enter unzip –help, and you’ll see something like the following image.
 
## Bzip2 for Zipping and Unzipping Files in Linux
 
Bzip2 is another compression utility built into most Linux distros. A major difference is that bzip2 cannot zip multiple files into one archive. Each file gets its own zipped archive.
 
### Zip Files in Linux Terminal With Bzip2
 
Enter the command bzip2 -kv9 testfile1.txt testfile2.txt where bzip2 is the command.
 
-kv9 breaks down to k means keep the originals, v means verbose so we can see what’s happening, and 9 for the highest level of compression. You can choose between 1 and 9. The higher the level of compression, the longer zipping the files takes.
 
The output tells us more than zip does, but the end result is almost the same.
 
### Unzip Files In Linux Terminal With Bzip2
 
Enter the command bzip2 -kvd testfile.1.txt.bz2 testfile2.txt.bz2. The -kvd options break down as k for keep the archives, v for verbose output, and d for decompress.
 
You see the files being decompressed and known when it’s done.
 
To view the bzip2 options, enter bzip2 –help, and you’ll see the following. Play around with the options on non-critical files just to see what they can do.
 
## Gzip for Zipping and Unzipping Files in Linux
 
This is the last of the popular compression utilities that are included with most distros. It’s lighter than bzip2 and zip for options. However, the quality of compression is still about the same.
 
### Zip Files in Linux Terminal With Gzip
 
Enter the command gzip2 -kv9 testfile.1.txt testfile2.txt. The -kv9 options break down as k for keep the files, v for verbose output, and 9 for the highest compression level between 1 and 9.
 
As the verbose output shows, gzip works about as well as the other zipping methods.
 
### Unzip Files in Linux Terminal With Gzip
 
There are two ways to unzip gzip archives. One is to use the gzip, and the other is gunzip.
 
For the gzip command, use gzip -kvd testfile1.txt.gz testfile2.txt.gz. Notice the d option. That means to decompress.
 
For the gunzip command, use gunzip testfile1.txt.gz testfile.2.txt.gz. The only difference from gzip is that gunzip doesn’t require options for a basic decompression.
 
## What About Tar to Zip and Unzip Files in Linux?
 
Why hasn’t tar been mentioned yet? It’s an archiving tool, taking a bunch of files and putting them into one archive for easy transport. Whatever the file sizes are, the size of the tar file will be about the same. 
 
But if you combine a zip method with tar, then you get something really cool. You get a nicely compressed single package of files. 
 
Using the other zip methods on a directory of files, you’d get a compressed archive for each file in the directory. Using tar with the gzip option on the directory compresses everything and makes one archive.
 
### Zip Files in Linux Terminal With Tar and Gzip
 
Enter the command tar -czvf Documents.tgz Documents. 
 
The -czvf options break down as c for create a new archive, z for compress with gzip, v for verbose output, and f for file equals archive, which means the archive maintains the file structure of the original directory. 
 
The new archive must be named, which is Documents.tgz in this example. By using the .tgz file extension, others will know that this is a tar archive that has been gzipped. Finally Documents is the directory to archive and compress.
 
The output looks like the following.
 
In File Manager, you can see the tar archive and that it’s compressed.
 
### Unzip Files in Linux Terminal With Tar and Gzip
 
To unzip a gzipped tar archive, it’s the same tar command with slightly different options. 
 
Enter the command tar -xzvf Documents.tgz Documents. 
 
The -xzvf options break down as x for extract, z for unzip with gzip, v for verbose so we can watch it happen, and f for file=archive means keep the file structure. Documents.tgz is the archive to be unpacked and unzipped, and Documents is the directory into which you want the contents to go.
 
The results are shown in the image below. The two files are back to full size, and they are in the Documents directory.
 
To view the tar options, enter tar –help, and you’ll get several pages of options. Notice that there are different zip methods available other than gzip, so you can choose the one you like.
 
## Less Popular Zip Tools in Linux
 
There are two more compression utilities found in most Linux distros. However, they’re not that popular. Nevertheless, they’re listed here, so you’re aware of them.
 
#### LZMA
 
LZMA is another command-line compression utility often found in Linux distros. It’s the compression algorithm used by 7-Zip.
 
#### XZ
 
The XZ utility is a command-line compression tool often included in Linux distros. Its options are similar to those of bzip2. It’s based on the LZMA2 algorithm, which is based on LZMA.
 
More information about these utilities can be found by using the commands lzma –help and xz –help.
 
## Aren’t There Other Ways To Zip and Unzip in Linux?
 
We’ve only gone into the compression tools built into most Linux distros. Still, Linux has several other ways to zip and unzip files. Some have GUIs, some are command-line utilities, and some can be used both with their GUI and through the command line. Do you use one of these zip tools in Linux? Which one is your favorite and why? Let us know in the comments.



