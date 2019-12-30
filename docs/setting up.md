---
menu: Setting Up HealthyPi v4
parent: getting-started.md
weight: 1
---

## Setting Up HealthyPi v4

Building upon its predecessor, HealthyPi v4 is enhanced to bring flexibility for end user's. Powered with popular esp32-wroom32 opens up the wireless and wearable capabilities. Now it's portable and standalone with in-built rechargeable battery.It can be used as HAT on raspberry or as a wearable platform.

### Setting Up HealthyPi v4 Complete Kit

The [HealthyPi v4 Complete Kit](https://www.crowdsupply.com/protocentral/healthypi-v4-unplugged#healthypi-v4-complete-kit) has all you need to quickly put together a standalone vital monitor. With the latest Raspberry Pi4 added with kit and microSD storage comes up with the HealthyPi v4 software pre-loaded and configured. Just Plug-in to stream live vital signs.

#### Simple Task in Complete Kit

The SmartiPi Touch Display that comes included with the HealthyPi v4 Complete kit is already partly assembled. Now it's time for you to take up the task by assembling the display enclosure and the display stand for the provided [SmartiPi Touch Case](https://smarticase.com/collections/all/products/smartipi-touch). Check out the below video for instructions on how to assemble the kit.

<iframe src="**assemble the kit**" width="640" height="360" frameborder="0" webkitallowfullscreen mozallowfullscreen allowfullscreen></iframe>


### Using HealthyPi v4 on Raspberry Pi

If you have a Raspberry Pi setup already available, just follow the following steps on your Raspberry Pi. You will need a monitor and a keyboard/mouse and the Raspberry Pi should be running Raspbian before proceeding with HealthyPi installation. To find out how to install Raspbian check out the simple tutorial on [Raspberry Pi's official site](https://www.raspberrypi.org/documentation/installation/noobs.md).

The following video shows you how to connect the HealthyPi v4 as **"HAT"** to a Raspberry Pi.

<iframe src="*HPi4 hat Rpi4*" width="640" height="360" frameborder="0" webkitallowfullscreen mozallowfullscreen allowfullscreen></iframe>

After completing the steps shown in the video, open up the terminal window (Menu -> Accessories -> Terminal) on Raspbian running on your Raspberry Pi:

![Open the terminal](images/terminal.jpg)

In the terminal window, type the following commands.

```bash
curl -sS http://pi.protocentral.com/hpi4.sh | sudo bash
```

Making the process even more simpler, this command will download and install all the required overlays, configuration and application files to get the HealthyPi v4 launched and running.

After the script reboots your Raspberry Pi, you should be able to see the GUI display the sensor outputs in real-time on the screen.

![GUI in Processing](images/hpi3-screen.jpg)

**This completes the install!**


## Getting started with the HealthyPi GUI on Windows, MacOS and Linux

The HealthyPi board now streams the same data on the on-board USB port. This allows you to get the same data that goes to the Raspberry Pi, now on your desktop PC as well.

<iframe src="https://player.vimeo.com/video/225754981" width="640" height="360" frameborder="0" webkitallowfullscreen mozallowfullscreen allowfullscreen></iframe>

*Java 8 is required on all platforms for running the processing-based GUI application. You can download Java for your platform from the following link.*

[https://java.com/en/download/](https://java.com/en/download/)

### Installing drivers (only for Windows)

HealthyPi uses the same drivers as an Arduino Zero. Once plugged in to the USB port, the device would be recognized as an "Unknown Device". You can locate the device is the Windows Device Manager and manually install the drivers provided in the "drivers" folder in the Windows Executable ZIP archive provided.

MacOS and Linux do not need any drivers to be installed.

### Processing GUI Installation

Download the zip file containing the executable files from the following links for 32-bit/64-bit Windows. If you do not know if you have a 64-bit or 32-bit computer, try with the 32-bit version.

[Download the latest release here](https://github.com/Protocentral/protocentral-healthypi-v3/releases/latest)

Simply download the appropriate file for your operating system, unzip the contents and run the executable program contained in it. On desktop operating systems, you will have to choose the correct port name assigned to the HealthyPi by USB. Simply select the port from the dropdown on the top and port should be opened.

*Note: On MacOS, if you see an error saying "app is damaged", please follow the steps given in https://support.apple.com/en-us/HT202491 .This is a known issue with Processing on MacOS.*