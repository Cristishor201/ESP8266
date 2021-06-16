# Prerequites

In order to can run Ubuntu, we need to install a linux environment, even for Linux itself. That's why we first will install Termux on the mobile phone.<br>
This is the only way I found without rooting your phone.

**Step 1**<br>
Go to [https://play.google.com/store/apps/details?id=com.termux](https://play.google.com/store/apps/details?id=com.termux) and install *Termux* on your Android OS.
![android_1](https://github.com/Cristishor201/ESP8266/blob/main/installation/ubuntu-android/android_1.jpg)

**Step 2**<br>
Run Termux.

**Step 3**<br>
We will download a package manager.<br>

    pkg install proot-distro
	y


**Step 4**<br>
Install Ubuntu 20.04.<br>

	proot-distro install ubuntu-20.04


**Step 5**<br>
For open Ubuntu on Termux, run:<br>

	proot-distro login ubuntu-20.04

**Step 6**<br>
Update the packages.<br>

	apt-get update -y

**Step 7**<br>
It's time to create a new user, as we are not going to use root for secure purpose.<br>
Firstly let's install sudo command.<br>
For this type in this order:<br>

    su -
    apt-get install sudo -y

**Step 8**<br>
Create a new user.<br>

    sudo adduser cristishor

Choose a *password* for you, and then confirm it again. Also it will ask you to enter *your name* / full name, *room number*, *work phone*, *home phone*, and *other*.<br>
But I will put only my surname, and skip the rest.<br>
Finally type *y* than you confirm the information above.

**Step 9**<br>
Now give sudo right to the new user we just created.<br>
while you are in the root user, type:<br>

    nano /etc/sudoers

Use the arrows to move up and down.<br>
Then under the *User privilege specification* section, add:<br>

	cristishor ALL=(ALL:ALL) ALL

Then press `ctrl` + `o` for saving the file. Don't forget for pressing enter for override the file.<br>
And then `ctrl` + `x` for exit.


**Step 10**<br>
For more secure reason type a password for root superuser also, after:<br>

    passwd


## Obtional 1 - Using alias:

Every time you want to run ubuntu on your termux, you must to run `proot-distro login ubuntu-20.04`. This is a long text to memorise it and also type it. There may be a better way, by using alias.

**Step 1**<br>
For that you have to go back to termux.<br>
Type `exit` so you can exit from ubuntu.<br>
![android_2](https://github.com/Cristishor201/ESP8266/blob/main/installation/ubuntu-android/android_2.jpg)

**Step 2**<br>

	cd ~
	cd nano ../usr/etc/bash.bashrc


**Step 3**<br>
In the opened settings file type:<br>

	alias ubuntu='proot-distro login ubuntu-20.04'


Then press `ctrl` + `o` for saving the file. Don't forget for pressing enter for override the file.<br>
And then `ctrl` + `x` for exit.

**Step 4**<br>
Reload the shell with:<br>

	source ../usr/etc/bash.bashrc

**Step 5**<br>
Done it.<br>


## Obtional 2 - Shared folders:

If you want to access created files or folders inside termux or Ubuntu proot-distro on your android device, then this section is for you.

**Step 1**<br>
Go to [https://play.google.com/store/apps/details?id=nextapp.fx](https://play.google.com/store/apps/details?id=nextapp.fx) and install *FX File Explorer* on your Android OS.<br>
![android_3](https://github.com/Cristishor201/ESP8266/blob/main/installation/ubuntu-android/android_3.jpg)

**Step 2**<br>
Open *FX File Explorer*, and accept the License Agreement. Accept media permission. Then it will show up some presentation, you can watch it or skip it by pressing *back button*. It will prompt to buy the premium versson, but we will need only the free one.

**Step 3**<br>
Click on the 3 dots in the top right corner, and then select *Connect to Storage*.<br>
![android_4](https://github.com/Cristishor201/ESP8266/blob/main/installation/ubuntu-android/android_4.jpg)


**Step 4**<br>
Click on the 3 horizontal bar in the top left corner, and then select Termux.<br>
![android_5](https://github.com/Cristishor201/ESP8266/blob/main/installation/ubuntu-android/android_5.jpg)

**Step 5**<br>
You can choose the home folder of termux, but I will create a new folder, by accessing again the 3 vertical dots in the top right corner, and then *Creat new folder*, give it a name, and then *Select* it.<br>
![android_6](https://github.com/Cristishor201/ESP8266/blob/main/installation/ubuntu-android/android_6.jpg)

**Step 6**<br>
For accesing a shared folder directly from ubuntu, you need to first create a folder on the android. For that go to *Main Storage* within **FX File Explorer**.<br>
Then select the 3 dots in the top right corner, and select *New* / *Folder*, and give it a name.<br>
I gave it `ubuntu-cristishor`.<br>
![android_7](https://github.com/Cristishor201/ESP8266/blob/main/installation/ubuntu-android/android_7.jpg)

**Step 7**<br>
Open termux, and run `ubuntu` or `proot-distro login ubuntu-20.04`.

**Step 8**<br>
Change the username we just created early with:<br>

    su - cristishor

**Step 9**<br>
Create a shorcut for the external folder we just created with:<br>

    ln -s /storage/emulated/0/ubuntu-cristishor /home/cristishor


## Obtional 2 - Tunneling with PC:

If you want to have both consoles side by side on the PC, you can acces the terminal from a desktop terminal.

First things first, you need to be already on ubuntu. If you are on termux, type again `proot-distro login ubuntu-20.04`.<br>

=============================================================

# Install & Configure Toolchain

Now it's time to install the actual tools to run & make builds.

**Step 1**<br>
Install prerequites by:<br>

	sudo apt-get install nano gcc git wget make libncurses-dev flex bison gperf python3 python3-serial
	y

**Step 2**<br>
Download the toolchain itself, for 64 bit verssion.<br>

	sudo wget https://dl.espressif.com/dl/xtensa-lx106-elf-gcc8_4_0-esp-2020r3-linux-amd64.tar.gz

**Step 3**<br>
Create a new folder, and extract the archive to it.<br>

	mkdir -p ~/esp
	cd ~/esp
	tar -xzf ../xtensa-lx106-elf-gcc8_4_0-esp-2020r3-linux-amd64.tar.gz
	
**Step 4**<br>
Download ESP8266_RTOS_SDK, by:<br>

	git clone --recursive https://github.com/espressif/ESP8266_RTOS_SDK.git

**Step 5**<br>
Open the `.profile` file, with:<br>

	sudo nano ~/.profile

And add these lines:<br>

	export PATH="$PATH:$HOME/esp/xtensa-lx106-elf/bin;/root/.local/bin"
	export IDF_PATH="$HOME/esp/ESP8266_RTOS_SDK"

Then press `ctrl` + `o` for saving the file. Don't forget for pressing enter for override the file.<br>
And then `ctrl` + `x` for exit.


**Step 6**<br>
Logout and then login again.<br>

	logout
	su - cristishor

**Step 7**<br>
If all are set corectly until this step, this command should print a long string link...<br>

	printenv PATH

and this one should print a short one.<br>

	printenv IDF_PATH

**Step 8**<br>
Install pip command.<br>

	sudo apt install python3-pip

**Step 9**<br>
Install required python packages:<br>

	sudo python3 -m pip install --user -r $IDF_PATH/requirements.txt

===================================

<s>
https://kinsta.com/knowledgebase/ssh-connection-refused/
https://linuxconfig.org/bash-netstat-command-not-found-debian-ubuntu-linux
https://kifarunix.com/allow-deny-specific-users-to-login-via-ssh-on-ubuntu-18-04/
https://johan.driessen.se/posts/Setting-up-an-SSH-tunnel-to-access-Remote-Desktop-using-Putty-and-SSHD-on-Linux/
https://askubuntu.com/questions/886313/what-is-the-simplest-way-to-have-remote-gui-access-to-ubuntu-16-04-server-from

https://www.cyberciti.biz/tips/ssh-public-key-based-authentication-how-to.html
https://www.tunnelbear.com/pricing
</s>

<s>(installation (download, prerequites, install | Configuring, issues case)
steps per sub-chapter</s>
