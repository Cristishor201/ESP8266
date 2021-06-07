# Prerequites

Before we start to install the OS, we need a couple of things first: to downoad it, and to write it on a DVD. There may be also to make a USB bootable, but for this tutorial I will cover only by CD (DVD). At least for now.<br>

**Step 1**<br>
Download ubuntu desktop from [here](https://ubuntu.com/download/desktop).<br>
This is what I installed: [Ubuntu 20.04.2.0 LTS](https://ubuntu.com/download/desktop/thank-you?version=20.04.2.0&architecture=amd64).

**Step 2**<br>
Go to [http://www.winiso.com/](http://www.winiso.com/) and download the free tool. This is the cheapest tool I found for burning bootable images to CD. In the following steps I will only how to burn normal CD, as I discovered it works aldo and it's free.

**Step 3**<br>
After installed it **WinISO**, open it.<br>
![os_1](https://github.com/Cristishor201/ESP8266/blob/main/installation/ubuntu-vBox/os_1.PNG)

**Step 4**<br>
Select Burn from the toolbar.

**Step 5**<br>
Next select the *CD/DVD/BD Recorder* from the drop-down list, and then click on the blue triangle to eject the tray.<br><br>
Insert a blank DVD, and put it back together.<br>
From the button with *...* browse the Ubuntu image we just downloaded.<br>
Then check in *Verification* and *Eject when finished*, and then begin the process of burning the DVD by pressing *Burn* button.<br>
![os_2](https://github.com/Cristishor201/ESP8266/blob/main/installation/ubuntu-vBox/os_2.PNG)

**Step 6**<br>
Insert the DVD in the PC where you want to install Ubuntu.

**Step 7**<br>
In order to boot from the DVD, instead of the hard drive, we need to go to BIOS and make a few changes there.<br>
In order to do that restart or turn on your computer. In the very begining press multimple times key *F2*. You should see a blue window like this one, in a short while.<br>
Go to *Boot* tab, and then select *Boot Device Priority*. For that use arrows to navigate through menu, and to make selection press *Enter* key.<br>
![os_3](https://github.com/Cristishor201/ESP8266/blob/main/installation/ubuntu-vBox/os_3.jpg) 

**Step 8**<br>
In the next window, give to your *CD/DVD reader* a greater priority than *SATA hardrive*. In this example I put the *DVD reader* into the first place, and *SATA hardrive* anywhere after it. To change position use *+* or *-*.<br>
After all is set, press *F10* key for save and exit, and then *Enter* key for *OK*.<br>
![os_4](https://github.com/Cristishor201/ESP8266/blob/main/installation/ubuntu-vBox/os_4.jpg) 


# Installation

**Step 1**<br>
In the first step Ubuntu it loads, it will checkthe integrity of the DVD. You can skp it if you want, but I highly recommended it, for making sure that we do not encounter other errors later on.<br>
![os_5](https://github.com/Cristishor201/ESP8266/blob/main/installation/ubuntu-vBox/os_5.PNG)

**Step 2**<br>
Select your language, and then choose to *Install Ubuntu*. In my case I will choose *English*.<br>
![os_6](https://github.com/Cristishor201/ESP8266/blob/main/installation/ubuntu-vBox/os_6.PNG)

**Step 3**<br>
Live the layout of keyboard as default with both English (US). This is the default keyboard layout for myself. Later on you can add another one as you want.<br>
![os_7](https://github.com/Cristishor201/ESP8266/blob/main/installation/ubuntu-vBox/os_7.PNG)

**Step 4**<br>
If you not connected the computer with a internet acces through LAN, it will ask you to connect through wireless.<br>
If you encounter this window, check in *Connect to this network*, and then select your Wi-fi and press *Connect* button, and then enter your password.<br>
Then hit *Continue*.<br>
![os_8](https://github.com/Cristishor201/ESP8266/blob/main/installation/ubuntu-vBox/os_8.jpg)

**Step 5**<br>
Live it as default: choose *Normal installation*, and the option to *Download updates*.<br>
Hit again *Continue* button.<br>
![os_9](https://github.com/Cristishor201/ESP8266/blob/main/installation/ubuntu-vBox/os_9.PNG)

**Step 6**<br>
If you have already installed Ubuntu before, this window may appear.<br>
In this case I will erase everything and I will start over, by selecting *Erase disk and install Ubuntu*. Then press *Install Now*, and on the prompt choose *Continue*.<br>
![os_10](https://github.com/Cristishor201/ESP8266/blob/main/installation/ubuntu-vBox/os_10.jpg)

**Step 7**<br>
Choose your time zone by typing your city, and then choose from the suggested list. I am from Bucharest, so I will press *Continue*.<br>
![os_11](https://github.com/Cristishor201/ESP8266/blob/main/installation/ubuntu-vBox/os_11.PNG)

**Step 8**<br>
Then choose a *name* for the computer, a *computer's name* (how is this device seen by others), and a *username* and a *password*. I make my choice as you can see. Also I checked in *Log in automatically*, as I get bored to enter by so many times the password on Ubuntu, but you are free to pick up the other choice.<br>
![os_12](https://github.com/Cristishor201/ESP8266/blob/main/installation/ubuntu-vBox/os_12.PNG)

**Step 9**<br>
After installation is finished, press *Restart Now*.<br>
![os_13](https://github.com/Cristishor201/ESP8266/blob/main/installation/ubuntu-vBox/os_13.PNG)

**Step 10**<br>
Remove the *DVD/CD*, put the try back, and press *Enter* key for continue.<br>
![os_14](https://github.com/Cristishor201/ESP8266/blob/main/installation/ubuntu-vBox/os_14.PNG)

**Step 11**<br>
If it throw a crash like this one, power off it from the button, and then restart it.<br>
![os_15](https://github.com/Cristishor201/ESP8266/blob/main/installation/ubuntu-vBox/os_15.jpg)

**Step 12**<br>
Next connect your accounts. I will connect this time only the Ubuntu account, as I already have it. If you want to make one too, go to [ubuntu account](https://login.ubuntu.com/+login) on any device. And then Hit *Next* / *Skip*.<br>
![os_16](https://github.com/Cristishor201/ESP8266/blob/main/installation/ubuntu-vBox/os_16.PNG)

**Step 13**<br>
Livepatch give you the ability to update your OS, without the necesity to restart. For set it up, all you need to do is just press *Set Up Livepatch*, enter your credentials, and then Click *Continue* when it pop up a message that alert you the need of aving an Ubuntu one account.<br>
Enter once more your password for Ubuntu account, and then choose a password for the Licepatch.<br>
A message text should appear that *You're all set*. Click *Next* green to continue.<br>
![os_17](https://github.com/Cristishor201/ESP8266/blob/main/installation/ubuntu-vBox/os_17.PNG)

**Step 14**<br>
I chosed not sending informations, but you are free to do so.<br>
I checked *No, don't send system info*. Then Click *Next*.<br>
![os_18](https://github.com/Cristishor201/ESP8266/blob/main/installation/ubuntu-vBox/os_18.PNG)

**Step 15**<br>
You can skip the activation of Location, as it's not needed for this setup, but I will activated as I can use it elsewhere within Ubuntu.<br>
Hit *Next*.<br>
![os_19](https://github.com/Cristishor201/ESP8266/blob/main/installation/ubuntu-vBox/os_19.PNG)

**Step 16**<br>
We will skip the installation of the apps, by clicking on *Done*.<br>
![os_20](https://github.com/Cristishor201/ESP8266/blob/main/installation/ubuntu-vBox/os_20.PNG)


# Configuring



<s>(installation (download, prerequites, install | Configuring, issues case)
steps per sub-chapter </s>