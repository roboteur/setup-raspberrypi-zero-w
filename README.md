# RASPBERRY PI ZERO W (Hassle Free Setup)

## REMOTE DISPLAY AND CONTROL (SSH + VNC)

#### 1. Flash The OS Raspbian Lite
* Download Raspbian Buster With Desktop >> https://www.raspberrypi.org/downloads/raspbian/
* Download etcher for flashing >> Etcher: https://www.balena.io/etcher/ 
* Flash the OS to the SD card

#### 2. Boot Setup (SSH and Network)
* Add a blank file named ssh (no ext) >> Inside the "boot" drive
* Add a file wpa_supplicant.conf >> Inside the "boot" drive

#### 3. Default ID and Password
* Type passwd to change rpi password
* ID: pi | PW: raspberry
* $ raspi-config | Similar to BIOS Setup for a PC 

#### 4. Fire Up Pi Zero W
* $ ssh pi@raspberrypi.local or $ ssh pi@ipaddress
* $ ping raspberrypi.local
* You can start coding here even without setting up the display

#### 5. Setup Remote Display (VNC)
* In your PC download and install VNC >> https://www.realvnc.com/en/connect/download/vnc/
* In Raspberry Pi >> Interface Option >> VNC
* Change Pi Zero resolution in the ip-config (this fixed the display probem).

## LIST OF COMMANDS
* Shutdown | $ sudo poweroff
* Pi Setup | $ raspi-config

## ISSUES/PROBLEMS AND SOLUTIONS
#### VNC Doesn't Work
* Solution: Go to raspi-config and change resolution. 

#### Desktop Login Doesn't Work
* Accepts user and password but doesn't push through with the boot >> Maker sure you have flashed the "desktop" version.
