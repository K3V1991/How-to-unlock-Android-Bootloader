<p align="center"><img src="https://i.ibb.co/pj0Pnj7/ADB-and-Fastboot-Plus-Plus.png" width="200"></a>
<h1 align="center"><b>How to unlock Bootloader using Fastboot on Android</b></h1>
<br />


## Download/install ADB & Fastboot on your Computer:
1. Use SDK Platform Tools - [Android Developers](https://developer.android.com/studio/releases/platform-tools) 
2. Or use my Tool: ADB & Fastboot++ - [GitHub](https://github.com/K3V1991/ADB-and-FastbootPlusPlus)

## Enable OEM Unlock:
**Note: If this Option is not present on your Device, it's likely that your Device didn't ship with Android Marshmallow or higher. 
If the Option is present but grayed out, this means that your Bootloader cannot be unlocked**
1. On your Phone, go to Settings > About Phone. Find the Build Number and tap on it 7 times to enable Developer Options
2. Now enter System > Developer Options, then enable the switchand next to "OEM unlocking"

## Reboot your Phone to Bootloader:
**Note: This Process will vary depending on your Device**
1. For most Phones, start by powering your Device completely off
2. When the Screen goes black, press and hold the "Volume Down" and "Power Button" simultaneously, and keep holding them for about 10 Seconds. If that doesn't work, turn the Phone off, then press and hold the "Volume Down Button" from there plug a USB Cable into your PC, then simply wait a few Seconds.
If that still didn't work, try repeating the USB Cable Method, but this time use the "Volume Up Button"
3. You should be greeted by Android's Bootloader Menu
4. Make sure your Phone or Tablet is plugged into your Computer with a USB Cable. Leave the Device alone, as the Rest of the Work will be done on the Computer Side

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
4. You'll see a Message on your Android Device asking if you're sure. Make sure the "Yes" Option is highlighted, press the Power Button, then your Bootloader will unlock and your Phone reboots back into Fastboot Mode
5. Reboot Device:
```
fastboot reboot
```
During reboot, your Device will go through a Factory Reset and then finally boot into System.
Your Android Device's Bootloader is now unlocked