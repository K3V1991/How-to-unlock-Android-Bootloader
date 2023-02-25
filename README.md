<p align="center"><img src="https://github.com/K3V1991/How-to-unlock-Android-Bootloader/blob/main/Lock.png" width="200"></a>
<h1 align="center"><b>How to unlock Bootloader using Fastboot on Android</b></h1>
<br />

<p align="center">
<a href="https://ko-fi.com/k3v1991" alt="Ko-fi"><img src="https://img.shields.io/badge/Ko--fi-F16061?style=for-the-badge&logo=ko-fi&logoColor=white"> &emsp;
<a href="https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=HW8B98TVDLKWA" alt="PayPal"><img src="https://img.shields.io/badge/PayPal-00457C?style=for-the-badge&logo=paypal&logoColor=white"> &emsp;
<a href="https://github.com/K3V1991/Donate-Crypto/blob/main/README.md" alt="Crypto"><img src="https://img.shields.io/badge/Bitcoin-000?style=for-the-badge&logo=bitcoin&logoColor=white">
</p>
<hr />
<br />

## Requirements:
* Windows OS
* ADB & Fastboot++ - [GitHub](https://github.com/K3V1991/ADB-and-FastbootPlusPlus)
* USB Driver for your Device or Universal ADB Driver

## Enable Developer Options & USB Debugging:
1. Install the USB Driver for your Phone or Universal Adb Driver
2. On your Phone, go to Settings > About Phone. Find the Build Number and tap on it 7 times to enable Developer Options
3. Now enter System > Developer Options and find "USB debugging" and enable it
4. Plug your Phone or Tablet into the Computer and change it from "Charge only" to "File Transfer" Mode
5. On your Computer, browse to the Directory where you extracted/installed ADB & Fastboot++
6. Launch a Command Prompt with Open CMD.bat or ADB & Fastboot++ Shortcut
7. Once you’re in the Command Prompt, enter the following Command: 
```
adb devices
```
and hit Enter

8. System is starting the ADB Daemon (If this is your first Time running ADB, you will see a Prompt on your Phone asking you to authorize a Connection with the Computer. Click OK.).
9. Succesful enabled USB Debugging.

## Rebooting to Bootlaoder:
1. Enter the following Command and hit Enter:
```
adb reboot bootloader
```
The Device reboots

## Unlocking the Bootloader:
**Note: That this will wipe all Data on your Device**
1. Type the following Command, then hit Enter:
```
fastboot devices
```
Returns a Series of Letters and Numbers followed by the Word "fastboot" then your Device is connected properly

2. If your Device shipped with Lollipop or lower pre-installed, enter the following Command:
```
fastboot oem unlock
```
3. If your Device shipped with Marshmallow or higher, type the following Command, then hit enter:
```
fastboot flashing unlock
```
You'll see a Message on your Android Device asking if you're sure. Make sure the "Yes" Option is highlighted, press the Power Button, then your Bootloader will unlock and your Phone reboots back into Fastboot Mode

4. Reboot the Device to System:
```
fastboot reboot
```
During reboot, your Device will go through a Factory Reset and then finally boot into System.
Your Android Device's Bootloader is now unlocked
