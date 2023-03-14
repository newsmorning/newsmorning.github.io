---
title: "Unlock the Secret to Decrypting SSL with Wireshark - Your Step-by-Step HTTPS Decryption Guide!"
ShowToc: true 
date: "2023-03-10"
author: "Robert Nunez"
---
*****
# Unlock the Secret to Decrypting SSL with Wireshark: Your Step-by-Step HTTPS Decryption Guide!

In today's digital world, online security is critical. More and more websites are using SSL (Secure Sockets Layer) to protect their users' data. SSL encrypts the data passed between a website and the user's browser to prevent it from being intercepted by hackers. This encryption makes it challenging for network administrators to monitor and analyze the traffic between the browser and the website. Luckily, Wireshark can help.

Wireshark is a popular open-source network protocol analyzer that can capture and display network packets. It can help you troubleshoot network-related issues and identify security problems. In this article, we'll guide you through the process of decrypting SSL with Wireshark.

## Prerequisites

To follow this guide, you'll need:

- Wireshark
- A private key and a certificate chain for the SSL connection you want to decrypt. (Note: you must have access to the server's private key to do this.)

## Step 1: Capture the SSL Traffic

To start the SSL decryption process, you need to capture the SSL traffic using Wireshark. Here's how to do it:

1. Launch Wireshark.
2. Select the network interface you want to capture the traffic on.
3. Click the "Capture Options" icon (the gear icon) in the toolbar.
4. In the "Capture Options" window, enter the SSL port number (443) in the "Capture Filter" field.
5. Click the "Start" button to begin capturing the SSL traffic.

Now that you're capturing the SSL traffic, you need to configure Wireshark to decrypt it.

## Step 2: Configure Wireshark to Decrypt SSL

Wireshark can decrypt SSL traffic using the private key and certificate chain you obtained earlier. Here's how to configure Wireshark to decrypt SSL:

1. In Wireshark, click the "Edit" menu and select "Preferences."
2. In the "Preferences" window, expand the "Protocols" section and select "SSL."
3. Click the "Edit" button next to the "(Pre)-Master-Secret log filename" field and select a location to save the log file.
4. Check the "Enable SSL decryption" box.
5. Click the "+" button to add a new RSA key.
6. In the "SSL RSA keys list" window, click the "Browse" button and select the private key you obtained earlier.
7. Enter the server's IP address and the SSL port number (443) in the "IP address" and "Port" fields, respectively.
8. Click the "OK" button to save the RSA key configuration.

Now, Wireshark is configured to decrypt SSL traffic.

## Step 3: Decrypt the SSL Traffic

With Wireshark configured to decrypt SSL traffic, you can now view the decrypted traffic. Here's how:

1. Stop capturing the SSL traffic.
2. Open the SSL traffic capture file in Wireshark.
3. Locate an SSL packet in the capture file and select it.
4. Right-click the SSL packet and select "Follow" > "SSL Stream."
5. If everything is configured correctly, you should now see the decrypted SSL traffic in the "SSL Stream" window.

If you're having trouble decrypting the SSL traffic, try the following troubleshooting steps:

- Make sure you have the correct private key and certificate chain.
- Make sure the RSA key configuration is correct.
- Check the log file for any errors or warnings.

## Conclusion

In this article, we've shown you how to decrypt SSL traffic using Wireshark, step-by-step. Decrypting SSL traffic can be useful in troubleshooting network-related issues and identifying security problems. With Wireshark and a bit of configuration, you can easily unlock the secrets of SSL and see the unencrypted data traveling between the web server and client.

{{< youtube 5qecyZHL-GU >}} 




 
#### In this post we cover:
 
## What are Wireshark and SSL Encryption?
 
Using Wireshark, you can look at the traffic flowing across your network and dissect it, getting a peek inside of frames at the raw data.
 
SSL is an encryption protocol that operates on the Transport layer of the OSI model. It uses various encryption methods to secure data as it moves across networks. Note: In this guide, I’ll mostly be referring to SSL as a catchall term for SSL and TLS, its successor.
 
SSL encryption makes using Wireshark more challenging because it prevents administrators from viewing the data that each relevant packet carries. When Wireshark is set up properly, it can decrypt SSL and restore your ability to view the raw data.
 
Make sure you are using the latest stable version of Wireshark.
 
 
Wireshark
Download the latest stable version


 
See also: Wireshark Alternatives for packet sniffing
 
## Using a pre-master secret key to decrypt SSL and TLS
 
Using a pre-master secret key to decrypt SSL in Wireshark is the recommended method.
 
Your browser can be made to log the pre-master secret key, which Wireshark uses to decrypt SSL and TLS sessions.
 
Here are the steps to decrypting SSL and TLS with a pre-master secret key:
 
- Set an environment variable
 - Launch your browser
 - Configure Wireshark
 - Capture and decrypt the session keys

 
When you’re finished, you’ll be able to decrypt SSL and TLS sessions in Wireshark without needing access to the target server.
 
### Set a Windows environment variable
 
In Windows systems, you’ll need to set an environment variable using the Advanced system settings utility. This variable, named SSLKEYLOGFILE, contains a path where the pre-master secret keys are stored.
 
Start by right-clicking on My Computer, and selecting Properties from the menu. The System menu will open.
 
Next, click Advanced system settings on the list to the left. The System Properties window will open.
 
On the Advanced tab, click the Environment Variables button.
 
Click the New… button under User variables. You can also create the variable under System variables if you’d like to log SSL keys for every user on the system, but I prefer to keep it confined to my profile.
 
Under Variable name, type the following:
 
SSLKEYLOGFILE
 
In the Variable value field, type a path to the log file. You can also click the Browse file… button and specify the path using the file picker.
 
As a note, if you’re creating this as a system-wide environment variable, you’ll need to use appropriate wildcards or store the file in a place accessible by all users. For instance, you might choose %USERPROFILE%\App Data\ssl-keys.log or C:\ssl-keys.log.
 
Once you’ve finished, click OK and move to the next set of steps.
 
### Set a Linux or Mac environment variable
 
In Linux and Mac, you’ll need to set the SSLKEYLOGFILE environment variable using nano. In Linux, the variable is stored in ~/.bashrc. On the Mac, you’ll create the variable in the file  ~/.MacOSX/environment
 
Open a terminal and use this command in Linux:
 
nano ~/.bashrc
 
Open Launchpad, click Other, and launch a terminal to run this command in Mac OSX:
 
nano ~/.bash_profile
 
The following steps are the same for both operating systems.
 
At the end of the file, add this line:
 
export SSLKEYLOGFILE=~/.ssl-key.log
 
Press Ctrl+X, Y to save your changes.
 
Close the terminal window and open another to set the variable, then type the following to confirm it’s been set successfully:
 
echo $SSLKEYLOGFILE
 
After you execute the command, you should see output similar to the image above. /Users/comparitech/.ssl-key.log is the full path to my SSL pre-master key log. Note: You’ll want to make a note of yours, which will be different, to enter in Wireshark.
 
Now that the variable has been set, you can move on to the next set of steps.
 
### Launch your browser and check for the log file
 
Before you launch Wireshark and configure it to decrypt SSL using a pre-master key, you should start your browser and confirm that the log file is being used.
 
In order to populate the log, it’s important that you visit a site that has SSL enabled. I’m using my own Apache server for testing, but any site will work. One of the biggest benefits of using a pre-master shared key is you don’t need access to the server to decrypt SSL.
 
After you’ve visited a SSL-enabled website, check the file for data. In Windows, you can use Notepad. In Linux or Mac, use the following command:
 
cat ~/.ssl-log.key
 
On any operating system, your file should look like mine does above. After you’ve confirmed that your browser is logging pre-master keys in the location you selected, you can configure Wireshark to use those keys to decrypt SSL.
 
### Configure Wireshark to decrypt SSL
 
Once your browser is logging pre-master keys, it’s time to configure Wireshark to use those logs to decrypt SSL.

 
Open Wireshark and click Edit, then Preferences. The Preferences dialog will open, and on the left, you’ll see a list of items. Expand Protocols, scroll down, then click SSL.
 
In the list of options for the SSL protocol, you’ll see an entry for (Pre)-Master-Secret log filename. Browse to the log file you set up in the previous step, or just paste the path.
 
When you’ve finished setting the (Pre)-Master-Secret log filename, click OK and return to Wireshark. You’re ready to move on.
 
Related post: How to use Wireshark
 
### Capture the session and decrypt SSL
 
The final step is to capture a test session and make sure that Wireshark decrypts SSL successfully.
 
- Start an unfiltered capture session, minimize it, and open your browser.
 - Visit a secure site in order to generate data, and optionally set a display filter of ‘ssl’ to minimize the session noise.
 - Click on any frame containing encrypted data.

 
In my case, I’ll select one that contains HTTP traffic with text/HTML encoding, since I’d like to see the source code the web server is sending to my browser. But any encrypted transmissions that use a pre-master secret or private key will work with this method. That includes all data utilizing Perfect Forward Encryption (PFE) through Diffie-Hellman or comparable key exchanges.
 
Once you’ve selected an encrypted data frame, look at the Packet byte view, and specifically the tabs underneath the view. You should see an entry for Decrypted SSL data, among others.
 
You’ll notice that my session still looks like it’s full of garbage, and no HTML is visible. That’s because my web server (and most Apache servers) use GZIP compression by default.
 
When you click the Uncompressed entity body tab, which only shows up in this case with SSL decryption enabled, you can view the source code of the site. For instance, here’s the title element of the default Apache page in plaintext.
 
## Using an RSA key to decrypt SSL
 
You might have noticed earlier that Wireshark has a field that allows you to upload your RSA keys and use them to decrypt SSL. In practice, RSA key decryption is deprecated.
 
If you were previously using an RSA key to decode traffic, and it stopped working, you can confirm that the target machine is using Diffie-Hellman exchanges by enabling SSL logging.
 
To turn on logging, click Edit from the toolbar menu and select Preferences. Expand the Protocols menu item on the left and scroll down to SSL. From here, you can click the Browse button and set the location of your SSL log.
 
Once the location is set, all SSL interactions will be logged in the specified file.
 
Capture a session with your SSL-enabled host, then check the logs. Specifically, you should scroll until you find the frame that the TLS handshake was negotiated on. It’s likely that you’ll see a telltale DHE entry in the cipher string.
 
That means Diffie-Hellman key exchanges are enabled. In my case, Apache is specifically using Diffie-Hellman with elliptic-curve keys, which is denoted by the string ECDHE.
 
Scroll a little further and you’re likely to see that the master secret cannot be found.
 
If your logs look like that, and you can’t decrypt data using an RSA key, you have no choice but to switch over to the pre-master secret method above.
 
Since PFE is becoming standard practice, with TLSv1.3 likely forcing the issue, simple RSA key decryption is deprecated and should not be used.
 
## Wireshark makes decrypting SSL traffic easy
 
I really like the way Wireshark handles the SSL decryption process. Cryptography is complicated, and the standards are constantly changing to be more secure. But once Wireshark and your environment are set up properly, all you have to do is change tabs to view decrypted data. It doesn’t get any easier than that.
 
Related Posts:
 
- Fix Common WireShark Startup ” no interfaces found” Issue
 - Wireshark Cheat Sheet
 - How to run a remote packet capture with Wireshark and tcpdump
 - Identify hardware with OUI lookup in Wireshark

 
- Start a packet capture session in Wireshark.
 - In the top menu bar, click on Edit, and then select Preferences from the drop-down menu.
 - In the Preferences window, expand the Protocols node in the left-hand menu tree.
 - Click on SSL. The main panel of the window will show protocol settings.
 - Enter a file name and select a location for SSL debug file.
 - Click in RSA keys list and then select Edit and then New.
 - Fill out the information fields in the pop-up window: IP address, Port, Protocol (which will be HTTPS), Key File, and Password. Press OK.
 - Click OK in the Preferences screen.

 
The data field at the bottom of the main Wireshark page will show the decrypted contents of the packet.
 
- Client hello: sent from the client to the server and includes its supported cipher suites and TLS version compatibilities.
 - Server hello: sent from the server to the client in response. It contains a link to the server’s public certificate and a request for the same back from the client.
 - The browser validates the server certificate and if all is OK, sends a link to its own certificate.
 - The server checks out the client’s certificate. If all is OK, session establishment continues.




