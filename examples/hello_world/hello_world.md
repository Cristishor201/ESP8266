# Hello world
---

## Table of content

- For Ubuntu
- For [Ubuntu on VirtualBox](#ubuntu-vBox)
- For Ubuntu on Android

<br />
<!--<h1 id="ubuntu-directly">Ubuntu</h1>
This is the part with instruction about how to build, flash and display the program if you are running ubuntu os. It will print **hello world** on the console, once it is uploded to the board.-->

<h1 id="ubuntu-vBox">Ubuntu VirtualBox</h1>
This is the part with instruction about how to build, flash and display the program if you are running ubuntu on VirtualBox. It will print **hello world** on the console, once it is uploded to the board.

**Step 1**<br>
Run Oracle virtualBox, and then start the virtual machine, in the *Detachable Start* state.<br>
![vBox_1](https://github.com/Cristishor201/ESP8266/blob/main/installation/ubuntu-vBox/vBox_7.png)

**Step 2**<br>
Ater it is starting up, enter your credentials.

**Step 3**<br>
Change the directory to esp, with:<br>

	cd ~/esp

**Step 4**<br>
Copy the example with hello world, and then go inside it.<br>

	cp -r $IDF_PATH/examples/get-started/hello_world .
	cd hello_world/

**Step 5**<br>
Connect the board to PC.<br>
[poza]

**Step 6**<br>
If nothing happens, it's because you need to install the driver.<br>
For that go to 


<s>
instalat driverul la vBox
instalat driverul la linux directly?

https://docs.espressif.com/projects/esp8266-rtos-sdk/en/latest/get-started/index.html#build-and-flash
make menuconfig...</s>