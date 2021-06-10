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
