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

<s>(installation (download, prerequites, install | Configuring, issues case)steps per sub-chapter </s>