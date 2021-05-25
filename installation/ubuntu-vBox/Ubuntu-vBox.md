# Downloading

Well, first of all let's download [Oracle Virtual Box](https://www.virtualbox.org/wiki/Downloads). In my case I will use Widows host option.

Then download Ubuntu or Linux. Both Virtual Box and Ubuntu, should be free, so there it would not be any problem with the license stuff. In this example I will use [Ubuntu Server 20.04.2 LTS](https://releases.ubuntu.com/20.04.2/ubuntu-20.04.2-live-server-amd64.iso), but you are free to use [any Ubuntu version](https://ubuntu.com/download/server) you want.

# Prerequites

Now it's time to install and configure Virtual Box.
The process it's quite simple, but for the sake of it, I will put all the necessary details.

**Step 1**<br>
Run the installation of the virtual box. Click next.<br>
![vBox_1](https://github.com/Cristishor201/ESP8266/tree/main/installation/ubuntu-vBox/vBox_1.png)

**Step 2**<br>
Choose to take all options, and also pick the location where you want to install Virtual Box. I recommend you to install virtual box on the computer at least, and the OS on the hard drive. Also it's a best practice to use underline or dash instead white spaces.<br>
![vBox_2](https://github.com/Cristishor201/ESP8266/tree/main/installation/ubuntu-vBox/vBox_2.png)

**Step 3**<br>
On next step I choosed to uncheck the shorcut of Quick launch Bar, but you can checked up if you want.<br>
![vBox_3](https://github.com/Cristishor201/ESP8266/tree/main/installation/ubuntu-vBox/vBox_3.png)

**Step 4**<br>
Next step it's pretty step forward. All you have to to is to press *yes*,<br>
![vBox_4](https://github.com/Cristishor201/ESP8266/tree/main/installation/ubuntu-vBox/vBox_4.png)

**Step 5**<br>
and then press *install*.<br>
![vBox_5](https://github.com/Cristishor201/ESP8266/tree/main/installation/ubuntu-vBox/vBox_5.png)

**Step 6**<br>
After the installation occured, press *Finish*, with the Start option checked, as we continue the setup, in the next chapter.<br>
![vBox_6](https://github.com/Cristishor201/ESP8266/tree/main/installation/ubuntu-vBox/vBox_6.png)

# Setup virtual image

Now it's time to create a virtual machine with ubuntu os machine we downloaded early.

**Step 1**<br>
Click *New* button, for creating a new disk image.<br>
![vBox_7](https://github.com/Cristishor201/ESP8266/tree/main/installation/ubuntu-vBox/vBox_7.png)

**Step 2**<br>
Select a name for the image (*I choosed Ubuntu Server 20 LTS*), the location on the hard drive or external hard drive; For type choose *Linux*, and for version choose *Ubuntu (64 bit)*.<br>
![vBox_8](https://github.com/Cristishor201/ESP8266/tree/main/installation/ubuntu-vBox/vBox_8.png)

**Step 3**<br>
In the next window choose the RAM Memory. More that you allocate, faster guest macine will run. However you should keep some memory also for host machine.
In this example I will choose 3100 (3GB), as I think it's more than enough, that we will not have the GUI part of the Linux.<br>
![vBox_9](https://github.com/Cristishor201/ESP8266/tree/main/installation/ubuntu-vBox/vBox_9.png)

**Step 4**<br>
Select to *create a virtual hard disk now*. This will be the virtual image of the operating system.<br>
![vBox_10](https://github.com/Cristishor201/ESP8266/tree/main/installation/ubuntu-vBox/vBox_10.png)

**Step 5**<br>
And then choose virtualBox disk Image.<br>
![vBox_11](https://github.com/Cristishor201/ESP8266/tree/main/installation/ubuntu-vBox/vBox_11.png)

**Step 6**<br>
Always choose Dinamically allocated, as it save you hard disk space, which is not used by the guest os.<br>
![vBox_12](https://github.com/Cristishor201/ESP8266/tree/main/installation/ubuntu-vBox/vBox_12.png)

**Step 7**<br>
And finally, choose a limit of hard drive for ubuntu. This can be as higher as you want. You can change later the location of the image, but you can't choose to upgrade this limmit later.<br>
I will choose 50 GB, as is more than enough for this tutorial or any tools and installation there.<br>
![vBox_13](https://github.com/Cristishor201/ESP8266/tree/main/installation/ubuntu-vBox/vBox_13.png)

**Step 8**<br>
Now, go to setings for the image we just created..<br>
![vBox_14]((https://github.com/Cristishor201/ESP8266/tree/main/installation/ubuntu-vBox/vBox_14.png)

**Step 9**<br>
Under the Storage section, in the Controller: IDE section, with the Host drive E selected..<br>
![vBox_15](https://github.com/Cristishor201/ESP8266/tree/main/installation/ubuntu-vBox/vBox_15.png)

**Step 10**<br>
Choose to change the disc with the ubuntu image we just downloaded before. This will mount the image, so that installation can begin.<br>
![vBox_16](https://github.com/Cristishor201/ESP8266/tree/main/installation/ubuntu-vBox/vBox_16.png)

**Step 11**<br>
Then we can start the *Ubuntu Server 20 LTS*, in *Detachable Start* state.<br>
![vBox_17](https://github.com/Cristishor201/ESP8266/tree/main/installation/ubuntu-vBox/vBox_17.png)

# Installation

**Step 12**<br>
The actual installation begins. We are prompted to select our language. I will choose English for myself.<br>
![vBox_18](https://github.com/Cristishor201/ESP8266/tree/main/installation/ubuntu-vBox/vBox_18.png)

**Step 13**<br>
On next screen we can choose the layout of the keyboard. I will live it as it is.
![vBox_19](https://github.com/Cristishor201/ESP8266/tree/main/installation/ubuntu-vBox/vBox_19.png)

**Step 14**<br>
We don't need network connection between this computer and other computer, so we will skeep this step.<br>
![vBox_20](https://github.com/Cristishor201/ESP8266/tree/main/installation/ubuntu-vBox/vBox_20.png)

**Step 15**<br>
We will skip also the settings for proxy server.<br>
![vBox_21](https://github.com/Cristishor201/ESP8266/tree/main/installation/ubuntu-vBox/vBox_21.png)

**Step 16**<br>
Hit next when it asking for ubuntu archive mirror.<br>
![vBox_22](https://github.com/Cristishor201/ESP8266/tree/main/installation/ubuntu-vBox/vBox_22.png)

**Step 17**<br>
On the next screen we are asked if we want to use ubuntu on one disc or more. I will live it as default.<br>
![vBox_23](https://github.com/Cristishor201/ESP8266/tree/main/installation/ubuntu-vBox/vBox_23.png)

**Step 18**<br>
This is just a Summary of the installation. Hit *Done* for next, and on the prompt with confirmation of destructive action, choose *Continue*.<br>
![vBox_24](https://github.com/Cristishor201/ESP8266/tree/main/installation/ubuntu-vBox/vBox_24.png)

**Step 19**<br>
Choose a name for the *user name* of this OS, a *name for this "computer"*, a *username* and a *password*. It's a good habbit to fill up al the inputs here.<br>
![vBox_25](https://github.com/Cristishor201/ESP8266/tree/main/installation/ubuntu-vBox/vBox_25.png)

**Step 20**<br>
Check in option for *install OpenSSH server*, and hit *Done*.<br>
![vBox_26](https://github.com/Cristishor201/ESP8266/tree/main/installation/ubuntu-vBox/vBox_26.png)

**Step 21**<br>
Here you can install extra options feature. We can install them later, so we will skip this as well.<br>
![vBox_27](https://github.com/Cristishor201/ESP8266/tree/main/installation/ubuntu-vBox/vBox_27.png)

**Step 22**<br>
After installing everything, press *Reboot Now*.<br> 
![vBox_28](https://github.com/Cristishor201/ESP8266/tree/main/installation/ubuntu-vBox/vBox_28.png)

You may get error for removing optical drive. Hit enter anyway, for continue.

**Step 23**<br>
Then login with your credentials.
![vBox_29](https://github.com/Cristishor201/ESP8266/tree/main/installation/ubuntu-vBox/vBox_29.png)

## Obtional

This section is for accessing VM with SSH from the host OS. This is the only way if you want to use copy-paste between host and the guest.<br><br>

Press Machine/ ACPI Shutdown, if your virtual machine it's still running. This is the shut down for it.<br>
![vBox_30](https://github.com/Cristishor201/ESP8266/tree/main/installation/ubuntu-vBox/vBox_30.png)

And then restarted it by *Start/Headless Start*.

**Step 1**<br>
Go again in Settings for this image, but this time on Network section. NAT adappter should be checked in. Click on the Advanced to expand the settings.<br>
![vBox_31](https://github.com/Cristishor201/ESP8266/tree/main/installation/ubuntu-vBox/vBox_31.png)

**Step 2**<br>
Then press *Port Forwarding*. Click on plus icon to add a new rule for the tunnel. And then choose some name and values. As you can see I chosed port 2222 for host, and port 22 for guest. I choosed them as they are not so common ports allocated by other services.<br>
![vBox_32](https://github.com/Cristishor201/ESP8266/tree/main/installation/ubuntu-vBox/vBox_32.png)

**Step 3**<br>
Download PuTTY from [here](https://www.chiark.greenend.org.uk/~sgtatham/putty/latest.html). I have Windows 64 bit version, so I will use  [putty-64bit-0.75-installer.msi](https://the.earth.li/~sgtatham/putty/latest/w64/putty-64bit-0.75-installer.msi). Installed it by going fast through the installation process. All I did here, is just checked in the desktop shorcut for it.

**Step 4**<br>
Start the PuTTY. And setup a new connection, but adding *localhost* on Host Name *2222* for the host port of local machine, and save this connection as *Ubuntu vBox*.<br>
![vBox_33](https://github.com/Cristishor201/ESP8266/tree/main/installation/ubuntu-vBox/vBox_33.png)

**Step 5**<br>
Open the connection with PuTTY. It may pop out a Security Alert window, but we trust the virtual machine we just installed, so we will accept it.<br>
If it crush, just restart the PuTTY.<br>
![vBox_34](https://github.com/Cristishor201/ESP8266/tree/main/installation/ubuntu-vBox/vBox_34.png)

**Step 6**<br>
Just login with your credentials, and you are good to go. 




<s>(installation (download, prerequites, install | Configuring, issues case, Install & configure toolchain + cod)
steps per sub-chapter</s>