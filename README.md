# [POCOX3-Root](https://github.com/blanckth/POCOX3-Root/)
## Full Root and TWRP recovery for POCO x3 pro
> ### Authur : **`Salar Muhammadi`**.
##### ##### ##### ##### ##### ##### ##### ##### ##### ##### ##### ##### #####
#### Download Repos and Essential Websites
##### Download [MIUI UNLOCK TOOL](https://en.miui.com/unlock/download_en.html)
##### Download [MIUI FASTBOOT FLASH TOOLs and ROMs](https://c.mi.com/oc/miuidownload/detail?guide=2) 
##### Download [TWRP APP](https://play.google.com/store/apps/details?id=me.twrp.twrpapp)
##### Download [TWRP IMG](https://dl.twrp.me/vayu/)
##### Download [MAGISK](https://magisk.me/apk/)
> ###### Tips : You can use this file for `rooting` the device as `Magisk-v23.0.apk` or rename it and flash with custom recovery (TWRP)
> ###### as `Magisk-v23.0.zip` for `rooting` and as `uninstall.zip` for `unroot`
##### Download [Universal ADB Drivers](https://adb.clockworkmod.com/)
##### Download [Platform-Tools](https://developer.android.com/studio/releases/platform-tools)
##### Download [Arrow OS](https://arrowos.net/download/vayu)
##### Download [LineAge OS](https://download.lineageos.org/vayu)
##### Download [NetHunter ARM64](https://www.kali.org/get-kali/#kali-mobile)
##### ##### ##### ##### ##### ##### ##### ##### ##### ##### ##### ##### #####
#### Special Boot Modes 
1. **Recovery**: 
    - With the device powered off, hold **`Volume Up`** + **`Power`**. 
    - When POCO splash appears, release ~~`Power`~~ and keep pressed **`Volume Up`** until recovery appears.
2. **FastBoot**:
    - With the device powered off, hold **`Volume Down`** + **`Power`**.
    - Keep holding both buttons until the word “FASTBOOT” appears on the screen, then release.
##### ##### ##### ##### ##### ##### ##### ##### ##### ##### ##### ##### #####
#### Prepration
- To use adb with your device, you’ll need to enable developer options and USB debugging:
    1. Open Settings, and select “About”.
    2. Tap on “Build number” seven times.
    3. Go back, and select “Developer options”.
    4. Scroll down, and check the “Android debugging” or “USB debugging” entry under “Debugging”.
    5. Plug your device into your computer.
    6. On the computer, open up a terminal/command prompt and type adb devices.
    7. A dialog should show on your device, asking you to allow usb debugging. Check “always allow”, and choose “OK”.
- Extract Platform-Tools to a path in Windows Drive like C:\platform-tools then exec this command in CMD :
    ```CMD
    setx /M path "%path%;C:\platform-tools\"
    ```
- Unlocking Bootloader
    1. Create a Mi account on [Xiaomi’s website](https://global.account.xiaomi.com/pass/register).
    2. Add a phone number to your Mi account.
    3. Insert a SIM into your phone.
    4. Enable developer options in Settings > About Phone by repeatedly tapping MIUI Version.
    5. Link the device to your Mi account in Settings > Additional settings > Developer options > Mi Unlock status.
    6. Run the [MIUI UNLOCK APP](https://en.miui.com/unlock/download_en.html) and follow the instructions provided by the app
        > NOTE: The app may tell you that you have to wait up to 30 days. If it does so, please wait the quoted amount of time before continuing to the next step.
    7. After device and Mi account are successfully verified, the bootloader should be unlocked.
    8. Since the device resets completely, you will need to re-enable USB debugging to continue.
##### ##### ##### ##### ##### ##### ##### ##### ##### ##### ##### ##### #####
```CMD
> adb devices
> adb reboot bootloader
> fastboot devices
> fastboot flash recovery twrp.img
> fastboot reboot
```
> ###### Be Patience...

#### Enjoy!
