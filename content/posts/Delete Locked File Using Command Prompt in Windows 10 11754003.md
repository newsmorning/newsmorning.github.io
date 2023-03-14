---
title: "Unlock the Secret to Deleting Stubborn Files in Windows 10 and 11 with This Command Prompt Trick!"
ShowToc: true 
date: "2022-12-28"
author: "Kenneth Sensabaugh"
---
*****
Unlock the Secret to Deleting Stubborn Files in Windows 10 and 11 with This Command Prompt Trick!

Are you tired of encountering stubborn files that simply refuse to be deleted in Windows 10 or 11? If you've tried everything from using the delete button to moving the file to the Recycle Bin and emptied it but still can’t delete them, then you're not alone. Fortunately, there is a hidden feature in the Windows operating system that can solve this problem with ease.

The good news is, you can use Command Prompt to delete those stubborn files that can't be deleted through the conventional methods. The Command Prompt allows users to apply advanced commands to perform various functions, including deleting stubborn files.

Here's how to do it:

Step 1: Open Command Prompt

Open your Windows Start menu or press the Windows key, then search for "Command Prompt." Once it appears on the results, click on it or select "Run as Administrator" to execute it as an admin.

Step 2: Locate the stubborn file

In the Command Prompt window, navigate to the folder or directory where the stubborn file is located. To do this, enter the "cd" command followed by the folder path, e.g., "cd C:\Users\YourUserName\Desktop" (replace "YourUserName" with your username and "Desktop" with the folder name).

Step 3: Identify the file's name

Type "dir /x" and press Enter. This command will display a list of all files and folders in the directory, including the 8.3 file name format of each file. Look for the file name you want to delete and take note of its 8.3 name. This name usually starts with a tilde (~) and is followed by the first six characters of the file's name.

Step 4: Use Command Prompt to delete the file

Type "del" followed by the 8.3 file name of the stubborn file and press Enter. For example, if the stubborn file's name is "StubbornFile.txt," and its 8.3 name is "~STUBBO," type "del ~STUBBO" and press Enter.

If the file is currently being used by another program or process, the Command Prompt will display an error message stating that the file cannot be deleted. In such cases, close any programs that are currently using the file and perform the delete command again.

That's it! You've successfully deleted the stubborn file using Command Prompt. The next time you encounter a stubborn file that refuses to be deleted, remember this trick.

Final Thoughts

Knowing how to use Command Prompt to delete stubborn files in Windows can save you a lot of time and frustration. While this method is useful, it should be used with care as it can delete files that are important to the operating system, which may cause issues. So, make sure you know what you're doing before using this method.

{{< youtube Qjbez66BVgg >}} 




 
## Delete Locked File Using Command Prompt
 
In general, Windows 10/11 comes up with “File in Use” or “File is Locked for Editing” error, if any User tries to delete a Shared File while it is still being used by another User.
 
In certain cases, Windows operating system can prevent a File/Folder from being deleted, even if the File/Folder was created by a User having full rights or permission to View, Edit and Delete Files.
 
In such cases, you should be able to delete the Locked File or Folder using Command Prompt with Admin Privileges.
 
### 1. Delete File Using Command Prompt
 
Any File, located anywhere on the computer or the network can be deleted by running Del/FolderPath\FileName.extension Command in the Command Prompt window.
 
1. Right-click on the Locked File that you want to delete and select Properties option in the drop-down menu.
 
2. On Properties screen, switch to Details tab and note down the Folder Path.
 
In this case, the Locked File Test.rtf is located at Folder Path C:\Users\Username\Desktop.
 
3. Next, type CMD or Comm in the Search bar > right-click on Command Prompt in the search results and select Run as Administrator option.
 
4. On Command Prompt screen, type del FolderPath\FileName.extension and press the Enter key.
 
Once the Command is executed properly, the File will be immediately force deleted and removed from your computer.
 
### Delete Locked Folder Using Command Prompt
 
Any Folder located anywhere on the Computer or Network can be deleted by running rmdir /s /q FolderPath\FolderName Command.
 
1. Right-click on the Locked Folder that you want to delete and select Properties option in the drop-down menu.
 
2. On Properties screen, you will find the Folder path listed next to the Location Entry.
 
3. Next, open Command Prompt as Admin > type rmdir /s /q FolderPath\FolderName and press the Enter Key.
 
Once the Command is executed, the Folder will be immediately Force Deleted and removed from your computer
 
- How to Change Ownership of File or Folder in Windows 10
 - Change Windows 10 Password Using Command Prompt




