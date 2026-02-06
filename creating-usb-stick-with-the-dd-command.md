# The dd command

DD is on every Linux and works the same way on all of them. First,
verify the dev name for your USB stick with the `lsblk` command.

```bash
lsblk # or
lsblk -o NAME,FSTYPE,MOUNTPOINT,SIZE

NAME   FSTYPE MOUNTPOIN   SIZE
sda                     894,3G
├─sda1 vfat   /boot/efi   976M
├─sda2 swap   [SWAP]     15,3G
├─sda3 ext4   /          74,7G
└─sda4 ext4   /home     803,4G
sdb                     115,6G
└─sdb1 vfat             115,6G
sr0                      1024M
```

The following command creates a USB installation stick and shows its
progress:

```bash
sudo dd status=progress if=.iso-file of=/dev/sdb
```

DD is short for *Disk Duplicator*. See also `man 1 dd`.
