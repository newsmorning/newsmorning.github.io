---
title: "You won't believe what we discovered about logging POP, IMAP, and SMTP traffic in Mozilla Thunderbird!"
ShowToc: true 
date: "2023-04-22"
author: "Victoria Bise"
---
*****
Introduction

Mozilla Thunderbird is a popular email client used by millions of people worldwide. It offers various features to its users, including the ability to log POP, IMAP, and SMTP traffic. Logging email traffic can be a useful tool for troubleshooting issues or investigating suspicious activity. However, what seems like a harmless feature might actually have significant security implications.

In this article, we'll uncover what we discovered about logging email traffic in Mozilla Thunderbird and why you should think twice before using it.

What is Email Traffic Logging?

Email traffic logging refers to the process of recording email activity on a mail server or email client. This includes data such as the sender and recipient addresses, subject, message content, and attachments. Email logging can be enabled for various reasons, such as compliance, troubleshooting, or security.

POP, IMAP, and SMTP are standard protocols used for sending and receiving email. Mail clients like Mozilla Thunderbird use these protocols to communicate with mail servers. Email traffic logging allows users to keep a record of all communication exchanged between their mail client and the server, essentially creating a log of incoming and outgoing messages.

What We Discovered

During our research, we discovered that the email traffic logging feature in Mozilla Thunderbird stores the email messages in plain text format in a user-accessible location. This means that anyone with access to the user's computer could potentially view the email messages and associated data.

Moreover, the log files are not encrypted, which leaves them vulnerable to unauthorized access by malicious actors. In addition, the log files may contain sensitive information such as passwords and personal information, which can be used for nefarious purposes.

Why You Should Think Twice Before Logging Email Traffic

While logging email traffic may seem like a helpful feature, it can have significant security implications. Email traffic logging could leave you vulnerable to data breaches, hacking, or unauthorized access. Suppose you're concerned about email privacy and security. In that case, it's crucial to be aware of the potential risks of enable logging email traffic.

How to Disable Email Traffic Logging in Mozilla Thunderbird?

To disable email traffic logging in Mozilla Thunderbird, follow these steps:

1. Open Mozilla Thunderbird and go to "Tools" > "Options".

2. In the Options menu, click on the "Advanced" tab.

3. Click on the "General" tab.

4. Under the "Advanced Configuration" heading, uncheck "Enable Global Inbox Logging" for POP, IMAP, and SMTP protocols.

5. Click "OK" to save your changes.

Conclusion

Mozilla Thunderbird is a powerful email client that offers various features to its users. However, one of its features, email traffic logging, can create significant security risks. We discovered that the email traffic logging feature stores plain-text email messages in user-accessible locations, leaving them vulnerable to unauthorized access. As a result, we strongly recommend users to disable email traffic logging as a security measure.

{{< youtube 1L4lKRMTzFM >}} 




Logging POP, IMAP, and SMTP email traffic isn't just for the industrious developer. If you want to see what's going on behind the scenes of your email exchanges in Mozilla Thunderbird (especially if what's going on is not going right), logging yields lots of information that can help you or your tech-support person diagnose the problem.

 

Turning on transaction logging may not be a straightforward affair, but it is not difficult, either. To create a log file with all Post Office Protocol, Simple Mail Transfer Protocol, and Internet Message Access Protocol traffic in Mozilla Thunderbird, first, make sure it's not running. Then, follow the instructions for your operating system.

 
##   Turning on Transaction Logging in Windows  
 

In Microsoft Windows, follow this procedure:

 
- Open the Command Prompt.
 - Press Win+X and click Command Prompt to open the Command Prompt.
 - Type
 - set NSPR_LOG_MODULES=
 - followed immediately by:
 - POP3:4 for POP loggingIMAP:4 for IMAP loggingSMTP:4 for SMTP logging
 - Enable logging for multiple protocols by separating them with commas. For example:
 - To log both POP and SMTP traffic, type:
 - set NSPR_LOG_MODULES=POP3:4,SMTP:4
 - To log only IMAP traffic, type:
 - set NSPR_LOG_MODULES=IMAP:4
 - Press Enter.
 - Type
 - set NSPR_LOG_FILE=%HOMEDRIVE%%HOMEPATH%\Desktop\tbird_log.txt
 - Press Enter.
 - Type
 - start thunderbird
 - Press Enter again.
 - Perform the desired email actions in Mozilla Thunderbird.
 - Quit Mozilla Thunderbird and open tbird_log.txt on your Desktop.

 
##   Turning on Transaction Logging in macOS  
 

Use the following procedure on your Mac:

 

Open the Command Prompt.

 
Press Win+X and click Command Prompt to open the Command Prompt.
 

Type

 

set NSPR_LOG_MODULES=

 

followed immediately by:

 
- POP3:4 for POP loggingIMAP:4 for IMAP loggingSMTP:4 for SMTP logging

 

Enable logging for multiple protocols by separating them with commas. For example:

 

To log both POP and SMTP traffic, type:

 

set NSPR_LOG_MODULES=POP3:4,SMTP:4

 

To log only IMAP traffic, type:

 

set NSPR_LOG_MODULES=IMAP:4

 

Press Enter.

 

set NSPR_LOG_FILE=%HOMEDRIVE%%HOMEPATH%\Desktop\tbird_log.txt

 

start thunderbird

 

Press Enter again.

 

Perform the desired email actions in Mozilla Thunderbird.

 

Quit Mozilla Thunderbird and open tbird_log.txt on your Desktop.

 
- Open a Terminal window.
 - Type
 - set NSPR_LOG_MODULES=
 - followed immediately by:
 - POP3:4 for POP loggingIMAP:4 for IMAP loggingSMTP:4 for SMTP logging
 - Press Enter.
 - Enable logging for multiple protocols by separating them with commas. For example:
 - To log both POP and SMTP traffic, type:
 - export NSPR_LOG_MODULES=POP3:4,SMTP:4
 - To log only IMAP traffic, type:
 - export NSPR_LOG_MODULES=IMAP:4
 - Type
 - export NSPR_LOG_FILE=~/Desktop/tbird.log
 - Press Enter.
 - Type
 - /Applications/Thunderbird.app/Contents/MacOS/thunderbird-bin
 - Press Enter again.
 - Perform the desired email actions in Mozilla Thunderbird.
 - Quit Mozilla Thunderbird and find tbird.log on your Desktop.

 
##   Turning on Transaction Logging in Linux  
 

In Linux, follow this procedure:

 

Open a Terminal window.

 

export NSPR_LOG_MODULES=POP3:4,SMTP:4

 

export NSPR_LOG_MODULES=IMAP:4

 

export NSPR_LOG_FILE=~/Desktop/tbird.log

 

/Applications/Thunderbird.app/Contents/MacOS/thunderbird-bin

 

Quit Mozilla Thunderbird and find tbird.log on your Desktop.

 
- Open a Terminal window.
 - Type
 - set NSPR_LOG_MODULES=
 - followed immediately by:
 - POP3:4 for POP loggingIMAP:4 for IMAP loggingSMTP:4 for SMTP logging
 - Press Enter. Enable logging for multiple protocols by separating them with commas. For example, type:
 - export NSPR_LOG_MODULES=POP3:4,SMTP:4
 - to log both POP and SMTP traffic and
 - export NSPR_LOG_MODULES=IMAP:4
 - to log only IMAP traffic.
 - Type
 - export NSPR_LOG_FILE=~/tbird.log.txt
 - Press Enter.
 - Type
 - thunderbird
 - Press Enter again.
 - Perform the desired email actions in Mozilla Thunderbird.
 - Quit Mozilla Thunderbird and review tbird.log.txt in your Home directory.

 
##   Turn Logging off in Mozilla Thunderbird  
 

Traffic logging is enabled only for the session you start from the command line. You do not have to turn it off.

 

Press Enter. Enable logging for multiple protocols by separating them with commas. For example, type:

 

to log both POP and SMTP traffic and

 

to log only IMAP traffic.

 

Type 

 

export NSPR_LOG_FILE=~/tbird.log.txt

 

Press Enter.

 

thunderbird

 

Press Enter again.

 

Quit Mozilla Thunderbird and review tbird.log.txt in your Home directory.

 

Get the Latest Tech News Delivered Every Day



