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

    pkg install proot-distro -y


**Step 4**<br>
Install Ubuntu 20.04.<br>

	proot-distro install ubuntu-20.04


**Step 5**<br>
For open Ubuntu on Termux, run:<br>

	proot-distro login ubuntu-20.04

**Step 6**<br>
Update the packages.<br>

	apt-get update -y



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
Done it.


## Obtional 2 - Tunneling with PC:

If you want to have both consoles side by side on the PC, you can acces the terminal from a desktop terminal.

First things first, you need to be already on ubuntu. If you are on termux, type again `proot-distro login ubuntu-20.04`.<br>
![android_3](https://github.com/Cristishor201/ESP8266/blob/main/installation/ubuntu-android/android_3.jpg)

------------------------------

**Step 1**<br>
Firstly install openssh package on Ubuntu.<br>

	apt install openssh-server -y


**Step 2**<br>
Change the password for the root super user.<br>
```passwd```, then type your password, and once more to confirm it.

**Step 3**<br>
Open configuration file for ssh.<br>

	nano /etc/ssh/sshd_config


**Step 4**<br>
Then add the following lines somewhere.<br>

    Port 2222
    PermitRootLogin yes


Then press `ctrl` + `o` for saving the file. Don't forget for pressing enter for override the file.<br>
And then `ctrl` + `x` for exit.

**Step 5**<br>
Restart opnessh by:<br>

	service ssh restart

<s>
https://www.youtube.com/watch?v=fo4SZQng4qc - users is not in the sudoers
https://help.ubuntu.com/community/SSH/OpenSSH/PortForwarding
https://askubuntu.com/questions/886313/what-is-the-simplest-way-to-have-remote-gui-access-to-ubuntu-16-04-server-from
https://johan.driessen.se/posts/Setting-up-an-SSH-tunnel-to-access-Remote-Desktop-using-Putty-and-SSHD-on-Linux/ --------------------------- cel mai probabil

https://www.youtube.com/watch?v=N8f5zv9UUMI -mai intai
https://www.youtube.com/watch?v=UWPaw8xUmKc

shared folder ?
</s>

<s>(installation (download, prerequites, install | Configuring, issues case)
steps per sub-chapter</s>
