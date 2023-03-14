---
title: "STOP Struggling with Python Permission Denied Errors on Windows 11! Discover These 5 Proven Fixes NOW!"
ShowToc: true 
date: "2023-02-16"
author: "Marla Dickinson"
---
*****
# STOP Struggling with Python Permission Denied Errors on Windows 11! Discover These 5 Proven Fixes NOW!

As a Python developer on Windows 11, you may have encountered the infamous "Permission Denied" error while trying to create, read, or modify files and directories. This error occurs when your Python script or application lacks the required permissions to perform certain operations on your computer's file system. It can be frustrating, confusing, and time-consuming, especially when you're trying to get your code to work.

In this article, we'll explore five proven fixes to common Python Permission Denied errors on Windows 11. By following these simple steps, you'll be able to troubleshoot and overcome this issue, and focus on what really matters: writing elegant and powerful Python code.

## Fix #1: Run Python as Administrator

One of the quickest fixes for Permission Denied errors on Windows 11 is to run your Python script or application as an administrator. This grants your code access to system resources that may be restricted by default, such as certain directories or files.

To run Python as an administrator, simply right-click on the Python executable file (either python.exe or pythonw.exe) and select "Run as administrator" from the context menu. Alternatively, you can open the Command Prompt or PowerShell as an administrator and type `python` followed by the name of your script or application.

Keep in mind that running Python as an administrator may pose some security risks, especially if your code interacts with sensitive data or third-party libraries. You should only use this fix if you trust the source of your code, and if you're aware of the potential risks.

## Fix #2: Change File Permissions

Another solution to Permission Denied errors on Windows 11 is to change the permissions of the file or directory that your Python code is trying to access. By default, some files and folders may be read-only or restricted to certain users or groups, which can prevent your script or application from working as intended.

To change file permissions on Windows 11, follow these steps:

1. Right-click on the file or directory that your Python code is trying to access.
2. Select "Properties" from the context menu.
3. In the Properties window, click on the "Security" tab.
4. Click on "Edit" to change the permissions for the current user or group.
5. Check the box for "Full Control" to grant your code full access to the file or directory.
6. Click "OK" to save the changes.

If you're not sure which user or group your Python code is running as, you can check the value of the `os.geteuid()` function, which returns the effective user ID of the current process. You can also use the `os.chown()` function to change the ownership of a file or directory programmatically.

## Fix #3: Disable Antivirus or Firewall

Sometimes, Permission Denied errors on Windows 11 may be caused by your antivirus or firewall software blocking your Python code from accessing certain files or directories. This is particularly common with third-party libraries that require network access or system-level permissions.

If you suspect that your antivirus or firewall is causing Permission Denied errors, you can try disabling them temporarily to see if the problem goes away. Keep in mind that this may pose some security risks, especially if you're connected to the internet or downloading external packages.

To disable your antivirus or firewall on Windows 11, follow these steps:

1. Click on the Windows Start button and type "Security."
2. Select "Windows Security" from the list of results.
3. Click on "Virus & threat protection" or "Firewall & network protection" depending on which feature is causing issues.
4. Turn off the toggle switch for your antivirus or firewall.

Once you've disabled your antivirus or firewall, try running your Python code again to see if the Permission Denied error has been resolved. If so, you may need to configure your security software to allow your code to access certain files or directories, either by adding them to a whitelist or by enabling specific network ports or protocols.

## Fix #4: Use Relative Paths

Another common cause of Permission Denied errors on Windows 11 is using absolute paths instead of relative paths in your Python code. Absolute paths refer to a file or directory's location on your computer's file system from the root directory, whereas relative paths refer to a file or directory's location relative to the current working directory of your Python script or application.

Using absolute paths can be problematic, especially if your code is intended to be run on different machines or operating systems with different directory structures. This can lead to hard-to-debug errors and inconsistencies, especially if your code depends on third-party libraries or external resources.

To use relative paths in your Python code, follow these best practices:

1. Use the `os.getcwd()` function to get the current working directory of your Python script or application.
2. Use the `os.path.join()` function to build file paths and avoid hardcoding directory separators.
3. Use the `__file__` attribute to get the path of the current script or module, and use it as a reference point for relative paths.

By using relative paths, you'll make your Python code more portable, maintainable, and resilient to changes in the underlying file system. You'll also reduce the risk of Permission Denied errors caused by incorrect or inaccessible file or directory paths.

## Fix #5: Check File Locks

Lastly, Permission Denied errors on Windows 11 may be caused by file locks, which occur when a file or directory is already in use by another process or user. This can happen if you're trying to read or modify a file that is still open in another application or window, such as a text editor or a file explorer.

To check for file locks on Windows 11, you can use the `pypiwin32` package, which provides a set of tools and extensions for Windows-specific Python development. You can install this package using `pip` by running `pip install pypiwin32`.

Once you've installed `pypiwin32`, you can use the `win32file` module to check for file locks and release them if necessary. Here's an example code snippet:

```python
import win32file
import win32con

file_path = "C:\\path\\to\\your\\file.txt"
file_handle = win32file.CreateFile(file_path, win32con.GENERIC_READ, win32con.FILE_SHARE_READ, None, win32con.OPEN_EXISTING, 0, None)

try:
    win32file.LockFileEx(file_handle, win32con.LOCKFILE_EXCLUSIVE_LOCK, 0, -0x10000, win32file.PyOVERLAPPED())
    # Your code here
finally:
    win32file.UnlockFileEx(file_handle, 0, -0x10000, win32file.PyOVERLAPPED())
    win32file.CloseHandle(file_handle)
```

This code snippet tries to obtain an exclusive lock on the file specified by `file_path`, and releases the lock once your code finishes executing. This can help prevent Permission Denied errors caused by file locks, and make your Python code more robust and reliable.

## Conclusion

Python Permission Denied errors on Windows 11 can be frustrating, confusing, and time-consuming. But by following these five proven fixes, you'll be able to troubleshoot and overcome this issue, and focus on what really matters: writing elegant and powerful Python code.

Remember to run Python as an administrator, change file permissions, disable antivirus or firewall, use relative paths, and check file locks as necessary. These simple solutions can save you hours of debugging and frustration, and help you become a more productive and effective Python developer.

{{< youtube bBvIZqpp7DU >}} 



Python is a program designed for building websites, software, and more using a high-level programming language. However, users have recently reported receiving a permission denied error in Windows 11. Here’s how to fix PermissionError [Errno 13] Permission denied error in Python.
 
## Try these solutions to fix PermissionError [Errno 13] Permission denied
 
- If Python cannot locate a file or does not have the necessary permissions to open it, then the PermissionError: [Errno 13] Permission denied error may occur.Release 3.7 introduced Python into the Microsoft Store which can cause permission denied errors.The latest version of Python is 3.10.7 and is available for macOS, Linux/UNIX, and Windows 8 or newer.

 

 


 
- Download Restoro PC Repair Tool that comes with Patented Technologies (patent available here).
 - Click Start Scan to find Windows 11 issues that could be causing PC problems.
 - Click Repair All to fix issues affecting your computer's security and performance

 
- Restoro has been downloaded by 0 readers this month.

 
Because Python uses a general-purpose language, it can be used to build a variety of different types of programs rather than focusing on a specific variable. 
 
For those wanting to learn more about developing and coding, Python is one of the easiest programming languages to learn, making it perfect for beginners.
 
## Why do I get the permission denied error in Python?
 
Users encounter PermissionError: [Errno 13] Permission denied error if providing Python with a file path that does not have permission to open or edit the file. By default, some files do not allow certain permissions. This error may also occur if providing a folder rather than a file.
 
If the file is already being operated by another process, then you may encounter the permission denied error in Python. If you’re receiving the Python runtime error, we offer solutions for that as well.
 
## How do I fix the Python permission denied error in Windows 11?
 
### 1. Check file path
 
One of the main causes of PermissionError: [Errno 13] Permission denied is because Python is trying to open a folder as a file. Double-check the location of where you want to open the file and ensure there isn’t a folder that exists with the same name.
 
Run the os.path.isfile(filename) command replacing filename with your file to check if it exists. If the response is false, then the file does not exist or Python cannot locate it.
 
### 2. Allow permissions using chomd
 
If the file does not have read and write permissions enabled for everyone, then you may encounter the permission denied error in Python. Try entering the chomd 755 filename command and replace filename with the name of your file.
 
This command gives everyone permission to read, write, and execute the file, including the owner. Users can also apply this command to entire directories. Running the ls -al command will provide a list of files and directories and their permissions.
 
### 3. Adjust file permissions
 
- Navigate to the location of your file in file explorer.
 - Right-click on the file and select Properties.
 - Click the Security tab then select your name under Group or user names.
 - Select Edit and go through and check permissions.
 - Click Apply then OK.

 
Adjusting the permissions of the file that you’re trying to open will allow Python to read, write, and execute the file.
 
Some PC issues are hard to tackle, especially when it comes to corrupted repositories or missing Windows files. If you are having troubles fixing an error, your system may be partially broken. We recommend installing Restoro, a tool that will scan your machine and identify what the fault is.Click here to download and start repairing.
 
Expert tip:
 
SPONSORED
 
### 4. Turn off execution aliases
 
- Click on Start and open Settings (or press Windows + I).
 - Open Apps then select Apps & features.
 - Open the drop-down menu next to More settings.
 - Click App execution aliases.
 - Locate the two App Installers for python.exe and python3.exe and toggle both to Off.

 
Python was added to the Microsoft Store for version 3.7 which introduced permission denied errors because it created two installers: python.exe and python3.exe. Disabling the Microsoft Store versions of Python should fix the permissions denied error.
 
- Show All Apps by Default in Windows 11 Start Menu [2 Tips]
 - How to Enable or Disable Copy Paste in Application Guard
 - How to Hide a Partition in Windows 11 [Easy Steps]
 - Download & Install Intel Bluetooth Driver for Windows 11

 
### 5. Update Windows and drivers
 
- Click on Start and open Settings (or press Windows + I).
 - Scroll down and select Windows Update.
 - Perform any available updates.
 - Select Advanced options.
 - Under Additional options, click on Optional updates.
 - Run any driver updates.

 
If you’re suddenly encountering the Python permission denied error and none of the above solutions worked, then check for any Windows 11 updates and perform any available driver updates.
 
If this method didn’t work either, we recommend you use specialized driver update software, DriverFix.
 
DriverFix is a fast and automated solution for finding all outdated drivers and updating them to their latest versions. The installation process it’s fast and safe so no additional issues will occur. 
 
### What is the latest version of Python?
 
As of the release of this article, the latest version of Python is 3.10.7 which is available for Windows 8 and newer and is not compatible with older versions including Windows 7. Python supports Windows, macOS, Linux/UNIX, and more.
 
###  DriverFix 
 
  Fast and simple tool to maintain all drivers updated.  
 
However, If users want to use older versions of Python, they can access releases 2.7 and newer or they can download a specific version of a release.
 
If you want a quick way to open PY files on Windows 10 and 11, we offer a guide for that as well.
 
Hopefully, one of the above solutions helped you fix the Python permission denied error in Windows 11. Let us know in the comments which step worked for you or if you have any suggestions for a different solution.
 
If the advices above haven't solved your issue, your PC may experience deeper Windows problems. We recommend downloading this PC Repair tool (rated Great on TrustPilot.com) to easily address them. After installation, simply click the Start Scan button and then press on Repair All.
 
Still having issues? Fix them with this tool:
 
- open python files

 
Email * 
 

Commenting as .
Not you?

 
Comment 





