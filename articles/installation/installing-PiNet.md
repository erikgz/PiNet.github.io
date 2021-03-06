---
title: "PiNet, a centralised user accounts and file storage system for a Raspberry Pi classroom."
layout: article
---

Installing PiNet
---------------------
#### **Warning** - Make sure you are installing PiNet onto a fresh installation. **Do not** install PiNet onto an Ubuntu installation running other services as PiNet can not be easily uninstalled.   
   
Now you have an Ubuntu 16.04 server setup, it is time to actually install PiNet. PiNet is run through a terminal.
This allows you use it locally or even run the software over SSH!
Lets get started!

1.  Once the machine reboots, login with your credentials you set up
    earlier.   
    ![](/assets/images/image11.jpeg)

2.  Select the search button in the top left corner.   
    ![](/assets/images/install-pinet1.jpeg)

3.  Search for and select “Terminal”. You can also just hit Ctrl + Alt +
    T.   
    ![](/assets/images/install-pinet2.jpeg)

4.  You will then be presented with a terminal. PiNet runs inside a
    terminal window. You may find it useful to resize the terminal
    window to make it larger or put it in full screen.   
    ![](/assets/images/install-pinet3.jpeg)

5.  Enter ```wget --content-disposition http://bit.ly/pinetbeta```
    and hit enter. This downloads the PiNet script. The main script is called ```pinet```.    
    (note the all new PiNet Jessie is now available in [Beta for testing](../wheezy-jessie.html).)    
    ![](/assets/images/install-pinet4.jpeg)

6.  Once that completes, enter ```sudo bash pinet``` which will launch
    PiNet. A desktop icon will be created when the software installs but 
    you can always use this command to manually launch PiNet.   
    ![](/assets/images/install-pinet5.jpeg)

7.  Enter your password as the application must be run as administrator 
    (nothing will look like it is being entered, this is a Linux security feature so don't worry, it is being entered).   
    ![](/assets/images/install-pinet6.jpeg)   
          
9.  PiNet will offer to run a full install, select yes.  
    ![](/assets/images/install-pinet7.jpeg)   
    
10. PiNet supports importing user data from an older PiNet server. 
    See the [migration guide](../manage-users/migration.html) for details. Select No.   
    ![](/assets/images/install-pinet8.jpeg)   

10. Select which release channel you wish to use. If using in a production environment, it is recommended you
    select stable. If you wish to test out new bleeding edge features, select bleeding edge.   
    ![](/assets/images/install-pinet9.jpeg)   

9.  The install will take roughly 1-2 hours depending on processor speed
    and internet speed. Select ok and it will start the installation.
    You can now leave it to work.   
    ![](/assets/images/install-pinet10.jpeg)

10. Around 1-2 hours later, the extra software dialog will be displayed.
    Here you can select any additional software you with to install.
    Libreoffice can be useful for a classroom; it is a free full office
    suit, similar to Microsoft Office. You can also install a custom
    package from the software repositories if you know its full name.
    Once you have finished, select cancel (or finished) to move on.   
    ![](/assets/images/install-pinet11.jpeg)   
    ![](/assets/images/install-pinet12.jpeg)   

11. Select yes when asked if you are finished installing software.   
    ![](/assets/images/install-pinet13.jpeg)

14. You must decide if you need students to have Sudo access on
    the Raspberry Pi. If you intend to work with the GPIO pins on the
    Raspberry Pi they will need it. You can really easily later enable
    or disable Sudo use in the Manage-Users submenu in the main software
    options. If in doubt, is recommended to enable it by selecting yes.   
    ![](/assets/images/install-pinet14.jpeg)   

13. If using 2 network interface cards then check the IP address is
    correct. If you are only using 1 (most people), then the default
    will likely be correct. Select yes.   
    ![](/assets/images/install-pinet15.jpeg)   

12. The operating system will now be compressed. After every change made
    to the operating system, it must be recompressed which takes roughly
    5 minutes normally. Select ok.   
    ![](/assets/images/install-pinet16.jpeg)

15. PiNet installation is now complete. The server has generated an
    SD card image which is located in /home/YourUser/piboot.
    You need to copy these files onto a blank formatted SD card and
    connect the Raspberry Pi to the network.   
    ![](/assets/images/install-pinet17.jpeg)

16. You are recommended to check the Backup section of this manual on
    setting up an automatic backup of your students work to an external
    hard drive in case of hard drive failure.   

## Copying to SD card
Now that you have installed PiNet, you need to [copy the boot files to an SD card](sd-card-copy.html).
