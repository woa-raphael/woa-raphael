<img align="right" src="https://raw.githubusercontent.com/graphiks/woa-raphael/65c0ee06045c13d1ef0f5f88aa687c50274ef7f5/raphael.png" width="350" alt="Windows 11 Running On A Redmi 9T Pro">


# Running Windows on the Redmi K20 Pro / Mi 9T Pro

## Root guide

### Prerequisites
- [Magisk](https://github.com/topjohnwu/Magisk/releases/latest)

- [ADB & Fastboot](https://developer.android.com/studio/releases/platform-tools)

- [TWRP](https://dl.twrp.me/raphael/twrp-3.7.0_9-0-raphael.img.html)

##### Boot TWRP
> If your recovery has been replaced back to stock, flash it again in fastboot with:
```cmd
fastboot flash recovery path\to\twrp.img reboot recovery
```
##### Backing up your boot image
> Sometimes flashing Magisk can cause a bootloop. To fix this, you'll need to restore a boot.img backup.

Use the TWRP backup feature to make a backup of the boot partition.

##### Flashing Magisk
- Flash the magisk.apk (you may have to rename it to magisk.zip) and reboot your phone. 
- Once booted, locate the Magisk app and open it.
- Follow any instructions provided. Select the direct install method if you are provided with several methods.

Your phone will now reboot, and you have succesfully rooted it.

## Finished!
