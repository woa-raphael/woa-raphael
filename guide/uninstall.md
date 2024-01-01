<img align="right" src="https://raw.githubusercontent.com/graphiks/woa-raphael/65c0ee06045c13d1ef0f5f88aa687c50274ef7f5/raphael.png" width="350" alt="Windows 11 Running On A Redmi 9T Pro">


# Running Windows on the Redmi K20 Pro / Mi 9T Pro

## Uninstallation
> [!WARNING]
> DO NOT RUN ANY OF THESE COMMANDS, THIS GUIDE IS A COPY-PASTED PLACEHOLDER FOR A DIFFERENT DEVICE AND IS SUBJECT TO CHANGE (it will probably brick your phone)

### Why is this needed?
If you want to uninstall windows this is used instead of deleting partitions manually to avoid human error + writing a whole dedicated guide to just uninstalling.

If you want to relock your bootloader you'll need your partition table to be stock.

### Prerequisites

- [ADB & Fastboot](https://developer.android.com/studio/releases/platform-tools)
- [gpt_both0.bin](https://github.com/woa-vayu/Port-Windows-11-POCO-X3-Pro/releases/tag/binaries)

#### Uninstall instructions

##### Restore GPT
> Replace ```path\to\gpt_both0.bin``` with the path to the gpt_both0.bin file.

```cmd
fastboot flash partition:0 path\to\gpt_both0.bin
```

##### Erase userdata to avoid a bootloop and restore FS size
```cmd
fastboot -w
```
