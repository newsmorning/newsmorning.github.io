---
title: "Revolutionize your Linux System Monitoring with Logwatch: The Ultimate Tool You Didn't Know You Needed!"
ShowToc: true 
date: "2022-12-16"
author: "Jerry Sisk"
---
*****
Revolutionize your Linux System Monitoring with Logwatch: The Ultimate Tool You Didn't Know You Needed!

Are you tired of manually monitoring your Linux system log files and trying to detect any anomalies? Look no further than Logwatch, the ultimate tool for revolutionizing your Linux system monitoring.

Logwatch is a free and open-source tool that runs on any Linux-based operating system, including Ubuntu, CentOS, Debian, and more. It can be easily installed and configured to gather and analyze log data from various sources, including system logs, web server logs, application logs, and more.

Here are some of the benefits of using Logwatch for monitoring your Linux system:

1. Automated monitoring and analysis: Logwatch automatically collects and analyzes log data from multiple sources and provides you with a concise and easy-to-read summary report of any anomalies, errors, warnings, or security threats detected.

2. Scalable and customizable: Logwatch can be easily customized to meet your specific needs and can handle large amounts of log data. It can also be integrated with other tools, such as Nagios, to create a powerful system monitoring and management solution.

3. Increased security: Logwatch helps you detect potential security threats and vulnerabilities by monitoring system logs for suspicious activity or unauthorized access attempts. This helps you to stay ahead of potential security breaches and safeguard your system and data.

4. Time-saving: With Logwatch, you don't have to spend hours manually scanning through log files to identify issues. It provides you with a clear and concise report that can easily be shared with other team members or stakeholders.

5. Cost-effective: Logwatch is a free and open-source tool, which means you don't have to spend money on expensive proprietary monitoring solutions. It's also low-maintenance, which means you don't have to spend a lot of time and resources on configuring and maintaining the tool.

Logwatch is a versatile and powerful tool that can be used by system administrators, developers, and security professionals to monitor and manage their Linux-based systems effectively. Its automated monitoring and analysis capabilities, scalability, and customization options, increased security features, time-saving benefits, and cost-effectiveness make it the ultimate Linux system monitoring solution.

In conclusion, if you haven't already incorporated Logwatch into your Linux system monitoring strategy, you're missing out on an excellent tool that could significantly streamline your monitoring efforts and keep your system secure. Give it a try and revolutionize your Linux system monitoring today!

{{< youtube kZ5LhS6fThM >}} 



If you are a system administrator, you’d probably know the importance of log files as well as the pain one goes through while analysing them, especially when you are dealing with a busy server. Luckily there are certain tools that make life easy for you, and one of them is Logwatch, a command line tool for log analysing and reporting in Linux.
 
In this article, we will discuss the basics of this tool, along with the features it provides.
 
Note: All the examples discussed in this article are tested on Ubuntu 14.04 and GNU bash, version 4.3.11(1). Logwatch is available for most Linux distro though.
 
## Installation
 
The Logwatch command is found in the repository of most Linux distro and can be installed using the following command.
 
Ubuntu or Debian-based distro:
 
or 
 
for Centos, Fedora or Redhat-based distro.
 
You can also install it from source from its official project page.
 
## Logwatch
 
Logwatch is basically aimed at helping with system log management. It has the ability to go through your logs for a given period of time and make a report in the areas that you wish with the detail that you wish.  Here are some of the examples explaining its usage:
 
## Get information on everything
 
By default, the Logwatch tool analyses and reports logs related to a wide range of services. For example, here is the output when the command was run without any options:
 

 
As you can see, the output information is large and is not convenient enough to be viewed on the terminal screen. So, it’s best you redirect it to a text file for easy viewing.
 
The screenshot above should give you an idea about the kind of report Logwatch creates. The header present at the top gives you an abstract of the command’s default configuration. For example, the “Processing Initiated field” contains information on the date and time when the command was executed, the “Date Range Processed” field contains information on the time period of the logs analysed, the “Detail Level of Output” field contains information on the detail level of the report, and the last two fields contain information on output format and local host.
 
After all this information, the actual report begins, wherein logs are segregated on the basis of services. For example, the first service here is dpkg status, followed by Kernel, pam_unix, Connections, sudo, and more.
 
## Limit output to a particular service
 
If you want, you can limit the command’s output to a particular service. This can be achieved by using the --service option. Here is an example:
 
So you can see that the command produced a report specific to the pam_unix service only.
 
## Specify the detail level
 
The command also allows you to specify the detail level of the report using the --detail option. The argument to this option can be high, med, or low, which correspond to the integers 10, 5, and 0, respectively.
 
As is clear from the first example discussed in this article, the default detail level is 0. Here is the default output of the command for the Kernel service:
 
and here is the output when the detail level was explicitly set to 10 or high:
 
So you can see, as the detail level was increased from 0 to 10, the information produced by the command also increased.
 
## Specify a date-range
 
You can also specify a date range to process, which means you can give the command a time range from which to process log entries. This can be achieved by using the --range option. Common ranges are Yesterday, Today, and All. Here is an example:
 
## Send the report to an email address
 
Logwatch is also capable of mailing the report to a particular email address. This can be achieved by using the --mailto option. Here is an example:
 
The command above sent the report to an email account. You should probably check your Spam folder for the email as Gmail has marked it as Spam for my email account.
 
For more information on Logwatch, go through the command’s man page.
 
## Conclusion
 
If you’re looking for a command line tool that can scan system log files and present the information in a human readable form, try Logwatch. It can easily be considered as one of the most helpful command line tools for general purpose logfile parsing and filtering.
 
Himanshu Arora is a freelance technical writer by profession but a  software programmer and Linux researcher at heart. He covers software tutorials, reviews, tips/tricks, and more. Some of his articles have been featured on IBM developerworks, ComputerWorld, and in Linux Journal.
 
Our latest tutorials delivered straight to your inbox



