<img align="right" src="https://raw.githubusercontent.com/graphiks/woa-raphael/65c0ee06045c13d1ef0f5f88aa687c50274ef7f5/raphael.png" width="350" alt="Windows 11 Running On A Redmi 9T Pro">


# Running Windows on the Redmi K20 Pro / Mi 9T Pro

## Troubleshooting Issues


## Cannot mount the Windows partition in Android or WoA Helper doesn't work
> This is caused when you shut down Windows instead of restarting it.
- To solve this, boot to Windows and then press "restart", then as the screen shuts off boot to TWRP and from there load up Android.
> Alternatively, if you have already set up the Switch to Android app, simply use this to switch to Android.

## USB does not work
Enable USB host mode using the optional [post install guide](postinstall.md)

## Restoring the WiFi drivers
The wifi drivers are disabled due to some instabilities, altough they aren't that frequent and does not bother me. To reenable them, (assuming you have reached the Windows desktop) copy over the driver files to your windows partition (by using mass storage mode or some other way), then in the Windows desktop, go to the driver folder, then inside of it navigate to the following directory: components/QC8150/Device/Raphael/DEVICE.SOC_QC8150.RAPHAEL/Extensions/Subsystems/. From within that folder find a file called "raphael_subextscss.inf_". Rename that file to remove the "_" at the end. Open Device Manager. Click on the "Add drivers" button at the top (should be the 6th icon). Click on "Browse". Navigate to the previous folder and select the .inf file you have just renamed. Windows will install the wifi driver, then reboot. Wifi should now be working.

## DISM Error:87 The add-driver option is unkown
This usually means that you have an unclean Windows image with some other drivers. You need to get a clean Windows image, like the one in [this Google drive link](https://drive.google.com/drive/folders/1JEC2QhFTyZhnm4qdzeFANTmeqoDCbS1I?usp=drive_link). Use 22h2, because touch appears to be broken in 23h2.

## 0xc000021a BSOD
This usually means that winlogon.exe has failed, and you may need to reapply the Windows image.

## The computer restarted unexpectedly or encountered an unexpected error
If you stumble upon this error, you may need to redeploy the Windows image. Use the [reinstall guide](reinstall.md) for this.
> This error usually occurs when you get a BSOD while Windows is setting up. Altough this BSOD is very uncommon since the WiFi drivers are disabled by default, which may crash. 

## INACCESSIBLE_BOOT_DEVICE BSOD
This Blue Screen of Death likely means some broken driver installation. To fix this, reinstall the drivers using the [reinstall guide](reinstall.md).

## My screen is dimmer than before
A weird workaround for this... is to just press the power button to put the phone to sleep, and again to wake it. Just works for some reason.

