🧭 The goal of this guide is to explain every step of the process for building a Pwnagotchi device. While the overall process is not too difficult, many things can go wrong - and in my case, they did. I’ve included all the issues I faced and how I fixed them, so you can avoid the same problems.

I hope this guide is useful for anyone trying to build their own Pwnagotchi, and that it also serves as a reference for me in the future.

🚀 Let’s get started!

<br>
<br>

### 🧰 Hardware Required
To build your own Pwnagotchi, you’ll need the following components:

🖥️ E-Ink Display pHAT – 2.13" (250x122) <code style="color : grey"> - A low-power, black-and-white screen that displays the Pwnagotchi interface.</code>

🍓 Raspberry Pi Zero 2 W <code style="color : grey"> - The small but powerful single-board computer that runs Pwnagotchi.</code>

🔋 PiSugar 3 Battery<code style="color : grey">  - The battery that powers your Pwnagotchi on the go.</code>

💾 MicroSD Card <code style="color : grey"> - Used to store the Pwnagotchi operating system and data.</code>

🔌 Micro USB Cable <code style="color : grey"> - For charging, powering, or connecting to the Pi for setup.</code>

<br>

### 🛠️ Step 1: Attach the Screen to the Raspberry Pi

Now that you have all your hardware, it’s time to put everything together!


1. Align the pins: Carefully align the pins of the E-Ink Display  with the GPIO pins on the Raspberry Pi.


2. Attach the screen: Gently press the display onto the Pi's GPIO pins. Make sure it fits, but don’t force it.


⚠️ Important: Be extra careful not to bend the pins, as they can be easily damaged. If the connection doesn’t feel right, double-check the alignment before applying any pressure.

<br>

### 💾 Step 2: Flash the SD Card with the Correct OS

1.  Download and Install Raspberry Pi Imager
First, download the Raspberry Pi Imager Software from the official website: Raspberry Pi Imager. Install it on your computer after downloading. https://www.raspberrypi.com/software/

2.  Find the Correct OS
The original Pwnagotchi image is not compatible with the Raspberry Pi Zero 2 W. To solve this, we’ll use Jayofelony’s Pwnagotchi image, which works with the Pi Zero 2. https://pwnagotchi.org/3rd-party-images/index.html

3.  Prepare the SD Card
Insert your microSD card  into your computer. Make sure it’s properly formatted and ready for use.

4.  Launch Raspberry Pi Imager
Once the Imager software is installed, open it on your computer.

5.  Flash the OS onto the SD Card
   
<code style="color : grey">  Select the Raspberry Pi model: In Raspberry Pi Imager, first, select the Raspberry Pi model (Raspberry Pi Zero 2 W).</code>

<code style="color : grey">  Choose the OS: Click "Choose OS" and select Custom to use the image you downloaded.</code>

<code style="color : grey">  Select the SD Card: Click “Choose SD Card” and select the microSD card that you inserted.</code>

<code style="color : grey">  Write the OS: Click Write to begin flashing the OS onto the SD card. Wait for the process to finish, which may take a few minutes.</code>

#### ⚠️ Note - If you get an error about the content being different than the written image, make sure the SD card is properly formatted and try again.
<br>

### 🔌 Step 3: Insert the SD Card and Connect the Raspberry Pi
1. Insert the SD Card into the Raspberry Pi

<code style="color : grey">Take the microSD card you flashed earlier and carefully insert it into the microSD card slot on the Raspberry Pi Zero 2 W.</code>

2.  Connect the Raspberry Pi to Your Computer

<code style="color : grey">Use a micro USB cable to connect the Raspberry Pi to your computer. Be sure to use the middle micro USB port, as it’s used for both power and data transfer.</code>

3.  Look for the Green Light

<code style="color : grey">Once connected, you should see a green light appear on your Raspberry Pi. This indicates that it powered up and is ready for use.</code>

4.  Troubleshooting No Green Light ⚠️

<code style="color : grey">If there is no green light, it’s most likely that the firmware is corrupted, meaning the OS wasn’t properly flashed onto the SD card. In this case, try flashing the image again.</code>


5. Download Drivers for Your Pi
   
<code style="color : grey">Once the Raspberry Pi is connected to your computer, the computer will recognize it, but it might not know exactly what the device is. To fix this, we’ll need to install drivers.</code>

<code style="color : grey">Go to this link: Pwnagotchi New Guerilla Guide. https://github.com/Xyl0se/Pwnagotchi-new-guerilla-guide?tab=readme-ov-file#2-basic-connectivity-ssh-ftp-connection-sharing Under Step 2, point 2.1, download the RNDIS drivers for your operating system.</code>

<br>

### ⚙️ Step 4: Manually Install the Driver via Device Manager

Once the RNDIS drivers are downloaded:


🔍 Open Device Manager on your computer.


🔌 Look for the Raspberry Pi device (usually under Ports (COM & LPT)).


🖱️ Right-click the device and select Properties.


📁 Go to the Driver tab → click Update Driver → choose Browse my computer for drivers.


📂 Select Let me pick from a list of available drivers on my computer → click Have Disk.


🔎 Click Browse, find and select the RNDIS.inf file you downloaded.


✅ Click OK, then Next, and the driver should install successfully.

