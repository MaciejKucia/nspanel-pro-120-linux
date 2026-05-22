# nspanel-pro-120-linux

## Backing up

Connect to the PC using USB cable, install android SDK Platform Tools then run:

```
adb root
adb exec-out "dd if=/dev/block/mmcblk0 bs=4096k" > nspanel_backup.img
```

The whole mmc memory will be backed up.

That whole-disk image can be extracted using 7zip. 

Partition can further be explored using https://github.com/NoahDomingues/Android-IMG-Editor/releases
