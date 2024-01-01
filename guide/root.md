<img align="right" src="https://raw.githubusercontent.com/graphiks/woa-raphael/main/media/raphael.png" width="350" alt="Windows 11 Running On raphael">


# Running Windows on the Redmi K20 Pro / Mi 9T Pro

## Root guide

### Prerequisites
- [Magisk](https://github.com/topjohnwu/Magisk/releases/latest)

- [ADB & Fastboot](https://developer.android.com/studio/releases/platform-tools)

- [TWRP](https://github.com/graphiks/woa-raphael/releases/download/raphael-partitioning/twrp.img)

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
