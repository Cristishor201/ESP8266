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
```
pkg install proot-distro -y
```

**Step 4**<br>
Install Ubuntu 20.04.<br>
```
proot-distro install ubuntu-20.04
```

**Step 5**<br>
For open Ubuntu on Termux, run:<br>
```
proot-distro login ubuntu-20.04
```

**Step 6**<br>
Update the packages.<br>
```
apt-get update -y
```


## Obtional 1 - Using alias:

Every time you want to run ubuntu on your termux, you must to run `proot-distro login ubuntu-20.04`. This is a long text to memorise it and also type it. There may be a better way, by using alias.

**Step 1**<br>
For that you have to go back to termux.<br>
Type `exit` so you can exit from ubuntu.<br>
![android_2](https://github.com/Cristishor201/ESP8266/blob/main/installation/ubuntu-android/android_2.jpg)

**Step 2**<br>
```
cd ~
cd nano ../usr/etc/bash.bashrc
```

**Step 3**<br>
In the opened settings file type:<br>
```
alias ubuntu='proot-distro login ubuntu-20.04'
```

Then press `ctrl` + `o` for saving the file. Don't forget for pressing enter for override the file.<br>
And then `ctrl` + `x` for exit.

**Step 4**<br>
Reload the shell with:<br>
```
source ../usr/etc/bash.bashrc
```

**Step 5**<br>
Done it.
