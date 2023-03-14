---
title: "You Won't Believe How Easy It Is To Clear Your Printer Queue in Just 5 Simple Steps on Windows 10!"
ShowToc: true 
date: "2023-01-21"
author: "Gabrielle Newman"
---
*****
# You Won't Believe How Easy It Is To Clear Your Printer Queue in Just 5 Simple Steps on Windows 10!

Have you ever encountered a situation where you were unable to print a document because it was stuck in the printer queue? It's a frustrating experience, and it's one that many Windows 10 users have faced. Fortunately, clearing the printer queue is a simple process that can be accomplished in just five steps.

## Step 1: Open the Print Spooler Service

To begin, you need to access the Print Spooler Service, which is responsible for managing the print queue. There are two ways to open this service:

1. The first method is to type "services" in the search box and select the Services app from the results. Look for the Print Spooler Service in the list, right-click on it, and select "Stop."
2. The second method is to press the Windows key + R, type "services.msc" in the Run dialog box, and press Enter. This will bring up the Services window. Find the Print Spooler Service, right-click on it, and select "Stop."

## Step 2: Navigate to the Printer Spooler

Once you've stopped the Print Spooler Service, you need to find the printer spooler file location. To do this, follow these steps:

1. Open File Explorer.
2. Type "C:\Windows\System32\spool\PRINTERS" in the address bar and press Enter.
3. This will bring up the printer spooler folder. All print jobs that are stuck in the queue will be here.

## Step 3: Delete All Print Jobs

Now that you've found the printer spooler folder, you need to clear it of all the print jobs. To do this, simply select all the files in the folder and press the Delete key. If you receive a message saying that the files are in use, make sure the Print Spooler Service is stopped and try again.

## Step 4: Restart the Print Spooler Service

Once all the print jobs have been deleted, you need to restart the Print Spooler Service. To do this, follow the steps from Step 1, but instead of selecting "Stop," select "Restart."

## Step 5: Test the Printer

Finally, test the printer to ensure that it is working properly. Simply try printing a document and make sure it prints successfully. If it does, you've successfully cleared the printer queue!

## In Conclusion

Clearing the printer queue may seem like a daunting task, but it's actually quite simple. With just five steps, you can easily clear the queue and start printing again. Whether you're a home user or a business owner, this is an essential skill to have in your arsenal. So, the next time you encounter a stuck print job, don't panic – just follow these steps and you'll be back up and running in no time!

{{< youtube Zb3LPwNcxEg >}} 



When you print a document or picture, Windows places the document/picture in a queue, and it’s called the print queue. In short, a print queue is nothing but a list of document(s) waiting to print.
 
Windows 10 automatically clears the print queue when the printer completes all pending jobs.
 
At times, you might need to manually clear the print queue to resolve a stuck print job. Clearing a print queue is relatively easy in Windows 10. Use one of the given below methods to clear the print queue in Windows 10.
 
Method 1 of 5
 
## The easiest way to clear the print queue in Windows 10
 
Step 1: Look for the printer icon in the system tray area of the taskbar and then double-click on it to view pending printer jobs.
 









 
Step 2: Click the Printer menu and then click Clear All Documents to clear the print queue.
 
Method 2 of 5
 
## Clear print queue via Devices & Printers
 
Step 1: Type Devices and Printers in the Start menu or taskbar search field and then press Enter key to open Devices and Printers window.
 
Step 2: Right-click on your printer’s icon, click See what’s printing option to view all print jobs that are currently in the queue.
 
Step 3: Right-click on a print queue, and then click Cancel option to clear the particular print job from the queue.
 
To clear all print jobs from the queue, click the Printer menu and then click Cancel All Documents option.
 
Method 3 of 5
 
## Clear the print queue via the Settings app
 
Step 1: Open the Settings app and then navigate to Devices > Printers & scanners.
 
Step 2: Click on your printer to see the Open queue button. Click on the Open queue button to view all print queue jobs.
 
Step 3: Right-click on a print job and then click Cancel to clear it from the print queue. To clear all documents from the print queue at once, click the Printer menu and then click Cancel All Documents option.
 
Method 4 of 5
 
## Manually clear the print queue in Windows 10
 
Use this method if the print job got stuck in the queue, and you are unable to clear the queue by following the methods mentioned above.
 
Step 1: In the Start menu or taskbar search box, type services.msc and then press Enter key to open Services window.
 
Step 2: Here, look for Print Spooler service. Right-click on Print Spooler service and then click Stop option. Minimize the Services window.
 
Step 3: Open File Explorer and navigate to the following folder:
 
C:\Windows\System32\spool\PRINTERS
 
Where “C” is the driver letter of Windows 10 install drive. If you see a dialog with “You don’t currently have permission to access this folder” message, click the continue button to open up the PRINTERS folder. If you are not the admin, you might need to enter the password.
 
Step 4: Under the PRINTERS directory, you will see many files. Select all files and press the delete key to delete all files. This will clear the print queue. Click the Yes button if you see the confirmation dialog.
 
Step 5: Maximize the Services window, right-click on Print Spooler service, and click Start to start the service.
 
Method 5 of 5
 
## Use third-party tools to clear the ­print queue
 
Plenty of free tools out there to help you clear the print queue in Windows 10. Print Queue Cleaner, Print Service Manager, and PrintFlush are two free tools that you can use to clear the print queue in Windows 10.
 
And if you have issues with the printer, use the official printer troubleshooter in Windows 10.



