---
title: "Unlock Hidden Windows 10 Secret: Double Your Jump List Items Efficiently!"
ShowToc: true 
date: "2023-06-10"
author: "Tammy Bryant"
---
*****
# Unlock Hidden Windows 10 Secret: Double Your Jump List Items Efficiently!

Are you tired of only seeing a handful of items in your Windows 10 jump list? Do you wish that you could access more of your recently used files and folders with ease? Well, you're in luck because there's a hidden Windows 10 secret that allows you to double the number of jump list items!

Jump lists are menus that appear when you right-click an application in the taskbar or start menu. They allow you to quickly access recently used files, folders, and functions within an app. By default, Windows 10 only displays 10 recent items in the jump list. However, doubling this number is simple.

## Step 1: Open the Registry

Before we can unlock this secret, we need to access the Windows Registry. To do this, press the Windows key + R on your keyboard and type "regedit" into the Run dialog. Then, press Enter.

## Step 2: Find the Jump List Settings

Once you're in the Registry Editor, navigate to the following location:

```
HKEY_CURRENT_USER\SOFTWARE\Microsoft\Windows\CurrentVersion\Explorer\Advanced
```

Alternatively, you can paste the above path into the address bar at the top of the Registry Editor window and press Enter.

## Step 3: Create a New DWORD Value

Next, we need to create a new DWORD value called "JumpListItems_Maximum". To do this, right-click in the right-hand pane of the Registry Editor and select New -> DWORD (32-bit) Value. Name this new value "JumpListItems_Maximum" (without the quotes).

## Step 4: Modify the Value Data

Double-click on the "JumpListItems_Maximum" value that you just created to open its properties window. In the "Value data" field, enter the number of recent items that you want to display in your jump list. For example, if you want to double the default number of items, you would enter 20.

## Step 5: Save and Exit

Finally, click OK to save your changes and exit the Registry Editor.

## Conclusion

That's all there is to it! You can now enjoy a longer jump list with more of your recently used files and folders. Keep in mind that increasing the number of jump list items may affect your system's performance slightly, so it's best not to set it too high. However, doubling the default number is a safe and efficient way to access more of your important files and folders. Give it a try and see how much it improves your workflow!

{{< youtube Fg03d5A-0gY >}} 



In our previous article, we discussed clearing Jump Lists history in Windows 10. In this guide, we will talk about changing the default number of items in Jump Lists in the taskbar and Start menu of Windows 10.
 
As you might have discovered by now, Windows 10 displays up to ten items in the taskbar and Start menu Jump Lists. If you would like to see more items, say 15 items, in Jump Lists, you will be surprised to know that there is no setting offered in Windows 10 to change the default number of items in Jump Lists.
 
In Windows 7, we could easily change the number of recent items displayed in Jump Lists by navigating to Taskbar and Start menu properties. Since Microsoft has moved Start menu settings to the new Settings, there is no setting under Taskbar and Start menu Properties to change the number of items to display to in Jump Lists.
 









 
Every setting of the Windows operating system can be changed under Registry. You can change or increase the number of items in Jump Lists in Windows 10 by manually editing the Registry.
 
## Increasing Jump List items
 
Complete the given below directions to increase the number of items in Jump Lists in the taskbar and Start menu.
 
NOTE: We recommend you create a manual system restore point before editing the Registry. If something goes terribly wrong after editing the Registry, which is very unlikely, you can revert to the original settings by restoring your Windows 10 PC to an earlier date.
 
Step 1: Type Regedit in the Start menu or taskbar search box, and then press Enter key. Click Yes button when you see the User Account Control dialog.
 
Step 2: In the Registry Editor, navigate to the following key:
 
HKEY_CURRENT_USER\Software\Microsoft\ Windows\CurrentVersion\Explorer\Advanced
 
Step 3: On the right-side, look for an entry named JumpListItems_Maximum. If there is no such entry, you need to create one by right-clicking on the empty area, clicking New, clicking Dword (32-bit) Value, and naming it as JumpListItems_Maximum.
 
Step 4: Double-click on JumpListItems_Maximum, and set its value to 20 or 30. That’s it! You may close the Registry Editor now.
 
NOTE: As per our observation, it’s not possible to reduce the default number of items in Jump Lists by using this method. On our PC, even after we set the value data to 5, Windows 10 continued to display 10 items in Jump Lists. Do let us know if you managed to reduce the number of items by using this or any other method.



