---
title: "SHOCKING: Popular Webdev Tool's Debug Mode Reveals Sensitive Data For Hundreds Of Sites - EVEN President Trump's!"
ShowToc: true 
date: "2023-04-12"
author: "Estela Ramsey"
---
*****
+++
title = "SHOCKING: Popular Webdev Tool's Debug Mode Reveals Sensitive Data For Hundreds Of Sites - EVEN President Trump's!"
date = "2021-08-10"
author = "Your Name"
tags = ["Web Development"]
description = "A popular web development tool's debug mode has been found to expose sensitive data for hundreds of sites, including President Trump's. Learn more about this shocking discovery and how to protect your website from such vulnerabilities."

+++

In the world of web development, debugging tools are crucial to locate and fix errors in the code. However, a recent discovery has revealed that a popular web development tool's debug mode could be exposing sensitive data for hundreds of sites, including President Trump's.

The tool in question is known as "Xdebug," and it is used by developers to debug PHP applications. Xdebug allows developers to analyze and profile their code to find errors and performance issues. However, when Xdebug's default settings are enabled, it also outputs detailed diagnostic information, including the values of all variables in use, the current stack trace, and the file name and line number of the currently executing code.

While this detailed information is helpful for debugging purposes, it could also expose sensitive information, such as usernames, passwords, API keys, and other confidential data, if stored in the code or passed as a query parameter.

The discovery was made by researchers at GoSecure, who found that over 35,000 servers were exposed to some level of Xdebug output. These servers included popular websites such as the website of the British Embassy in Indonesia and the website of the Office of the Comptroller of the Currency. Even more alarming was the discovery that President Trump's official campaign website was also affected.

The researchers found that the Xdebug output from the Trump campaign's website contained sensitive information, including the email addresses, names, and location data of campaign donors. This information could be used by malicious actors for phishing attacks and identity theft.

The good news is that this vulnerability can be easily fixed by disabling Xdebug's default settings or restricting its output to localhost only. Developers can also use tools such as Git and Bitbucket to manage their code and ensure that sensitive information is not stored in the codebase.

Website owners and users can take some precautions to protect themselves from such vulnerabilities. They should only enter sensitive information on secure websites that use HTTPS and are certified by trusted authorities. Users should also avoid using the same passwords for multiple websites and enable two-factor authentication whenever possible.

In conclusion, the discovery of Xdebug's vulnerability should serve as a wake-up call for developers and website owners to take cybersecurity seriously. With the increasing threats of cybercrime, it is more important than ever to protect sensitive data and ensure that our websites are secure. By following best practices and keeping our software up to date, we can prevent such vulnerabilities and make the web a safer place.

{{< youtube 8gcu2GQf7PI >}} 




 
Hundreds of websites made using a popular web development tool have exposed sensitive data to anyone with a web browser. They include Donald Trump’s official campaign website, potentially allowing attackers to hijack the site’s email server.
 
The tool, a PHP framework called Laravel, includes a “debug mode” that lets developers identify errors and misconfigurations before websites go live. The problem is that many developers fail to disable the debug mode after going live, exposing backend website details like database locations, passwords, secret keys, and other sensitive info.
 
Comparitech worked with security researchers Bob Diachenko and Sebastien Kaul to uncover websites made vulnerable through Laravel’s debug mode and notify the owners of the exposures starting on October 11. They found 768 websites with active Laravel sessions in all, and he estimates 10 to 20 percent of them contain sensitive configurations. Most of the websites are for charities and small businesses.
 
A subdomain of Trump’s campaign website contained a mail server configuration exposed in plain text, visible from any web browser through the Laravel debug interface. It’s impossible for us to determine when debug mode was enabled, so we don’t know how long the data was at risk.
 
“Even 24 hours is dangerous enough,” Diachenko says. “Theoretically, anybody could use these credentials to impersonate the Trump campaign and send emails on behalf of email.donaldtrump.com.”
 
The potential consequences of such an exposure are quite serious; Trump’s campaign website is used to solicit donations, after all. Attackers could have intercepted correspondence with Trump supporters or phish campaign contributors, among other crimes.
 
To be clear, this is not a breach of user data; no user records were leaked. This exposure instead gave hackers an attack vector to potentially hijack mail servers, explore source code structure, find weak points, re-use passwords on other systems, and mount other types of attacks.
 
The DonaldJTrump.com team responded on October 16 and fixed the issue.
 
The FBI, Homeland Security, and the Office of the Director of National Intelligence coordinate to mitigate the risk of cyber influence operations targeting U.S. elections and provide presidential campaigns with defensive briefings.
 
## What is Laravel?
 
Laravel is a popular open-source PHP framework used to develop web applications. According to BuiltWith, more than 135,000 live websites currently use it.
Like similar frameworks, it includes a debug mode with an interface that allows developers to identify errors and misconfiguration on the site’s network. This debug mode is intended to be used before the site goes live, but many developers failed to disable it. To be clear, this is an error made by the site’s administrator or developer and not a bug in Laravel.
 
The debug interface can be accessed from a web browser. It often contains plain-text sensitive details and API credentials like shared secrets, passwords, and database locations—information that hackers can use to steal data or develop further attacks on the system.
 
This is not a new problem. About one year ago, Diachenko and his colleague Sebastien Kaul conducted an internet-wide search that found 566 public IP addresses with Laravel’s debug mode enabled. They notified 22 companies with exposed credentials. That included a Swedish company called PrestoDaycare, which makes digital classroom technology and child tracking software.
 
Exposed information through debug APIs is a common problem for websites using PHP frameworks, despite well-documented risks spanning back two decades.
 
## How and why we discovered this exposure
 
Comparitech’s security research team scans the internet for misconfigured websites and databases left exposed on the web. We make every attempt to alert the responsible organizations in order to minimize harm to end users.
 
Bob Diachenko leads our efforts using his extensive knowledge and experience in cybersecurity. The team then investigates what data was exposed, for how long, to whom it belongs, and who is affected.
 
We report the results to raise awareness among victims so they may take the necessary steps to protect themselves. Our aim is to stop unauthorized access to personal information and mitigate the harm that can result from such data exposures and breaches.
 
In the case of Trump’s campaign website, we made several attempts to notify the campaign. Here is the timeline of our efforts to make contact:
 
- 11 Oct – Diachenko contacted privacy@donaldtrump.com and
 - privacy@trump.com
 - 14 Oct – Submitted the DonaldJTrump.com contact form
 - 14 Oct – Emailed the info@ email address
 - 15 Oct – Emailed Brad Parscale (campaign manager) – email address found online
 - 15 Oct – Emailed America First Policies (info@ email address) to see if they have any contacts that could help
 - 15 Oct – Emailed privacy@trump.com (listed in privacy policy) again but this email bounced
 - 15 Oct – Submitted the Parscale Digital contact form. Brad Parscale is the founder of digital agency Giles-Parscale (now Parscale Digital) and sources suggest he may have built DonaldJTrump.com. We received an automated acknowledgement of our submission.
 - 16 Oct – Submitted a contact form for James P. O’Neill, the NYPD Police Commissioner. The form is on NYC.gov and we received an automated acknowledgement of receipt.
 - 16 Oct – Submitted the DonaldJTrump.com contact form again
 - 16 Oct – Emailed Parscale Digital using the info@ email address, which bounced
 - 16 Oct – Contacted the whois registrant email for DonaldJTrump.com
 - 16 Oct – Contacted the whois registrant email for parscaledigital.com
 - 16 Oct – Contacted Brad Parscale via LinkedIn
 - 16 Oct – Contacted Megan Powers (Director of Operations) via LinkedIn
 - 16 Oct – Contacted Dade Varsafsky (Office Manager) via LinkedIn
 - 16 Oct – issue fixed by Trump’s team

 
## Previous data breach and exposure reports
 
- 700,000 customer records for major hotel franchisor Choice Hotels
 - 7 million records of K-12 students
 - 188 million personal data records from people search sites
 - 300,000 records belonging to cryptocurrency exchange QuickBit
 - 5 million personal records belonging to MedicareSupplement.com




