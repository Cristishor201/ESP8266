# Downloading

Well, first of all let's download [Oracle Virtual Box](https://www.virtualbox.org/wiki/Downloads). In my case I will use Widows host option.

Then download Ubuntu or Linux. Both Virtual Box and Ubuntu, should be free, so there it would not be any problem with the license stuff. In this example I will use [Ubuntu Server 20.04.2 LTS](https://releases.ubuntu.com/20.04.2/ubuntu-20.04.2-live-server-amd64.iso), but you are free to use [any Ubuntu version](https://ubuntu.com/download/server) you want.

# Prerequites

Now it's time to install and configure Virtual Box.
The process it's quite simple, but for the sake of it, I will put all the necessary details.

## Install

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

# Installation

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


<s>(installation (download, prerequites, install | Configuring, issues case)
steps per sub-chapter</s>