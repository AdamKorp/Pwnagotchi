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
