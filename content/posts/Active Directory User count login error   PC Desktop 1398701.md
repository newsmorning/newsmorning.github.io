---
title: "You won't BELIEVE what happened when we found out our Active Directory User Count was giving us a Login Error on our PC Desktop!"
ShowToc: true 
date: "2023-04-12"
author: "John Ellison"
---
*****
Title: You Won't Believe What Happened When We Found Out Our Active Directory User Count Was Giving Us A Login Error on Our PC Desktop!

Introduction:

As IT professionals, we thrive on fixing unexpected technical glitches. But, what happens when the error is so bizarre that we are left scratching our heads? Recently, our team experienced just that when we encountered a login error on our PC desktops due to an issue with Active Directory User Count. Read on to find out how we tackled this unusual problem.

Background:

Active Directory User Count is an essential metric that helps IT professionals manage the number of users in the Active Directory domain. This count is typically used to optimize the Active Directory infrastructure, prevent license over-utilization, and provide a better user experience. However, it was causing a login error on our desktops, which was highly unusual.

The Problem:

One day, we received an avalanche of error messages from users attempting to log into their desktops. The error message read: "The system could not log you on. Make sure your username and domain are correct." After examining the event viewer logs of the affected machines, we noticed that the error was related to the Active Directory User count. We discovered that the Active Directory system was considering the inactive user accounts during the login process, hence causing the error.

The Solution:

To solve the problem, we had to update the Active Directory system with a script that excluded the inactive user accounts from the user count. We also removed the inactive user accounts from the domain to ensure that they did not affect the user count.

After updating and fixing the script, we tested the login process, and it worked without any issues. The error messages were no longer visible, and the users could log in with ease.

Conclusion:

It's always a fun adventure to solve a technical problem that doesn't fit the usual mold. Our team's mission is to investigate the cause, identify the strategy used, and come up with a solution that works. Fixing the login error due to Active Directory User Count was a fascinating and yet bizarre journey, much like unraveling a puzzle. Thankfully, our team was up to the task and solved the problem in no time.

{{< youtube udntF-jwiEE >}} 



## Chosen Solution
 Active Directory user account logs in fine on computers that have a user profile already but gives username or password incorrect when log on to a new computer to create a profile.

 Is the computer 1 connecting to DC correctly and has the most recent state of the user account?
Is the computer 2 connecting to the same DC as computer 1?
If they are connecting to different DCs, are they replicating correctly and have you given them enough time to replicate after password change?




