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

