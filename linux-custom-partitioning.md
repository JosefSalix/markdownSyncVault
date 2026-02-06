# How I prefer to setup linux workstations

| ==Partition== | ==Filesystem== | ==Mountpoint== |
|---------------|----------------|----------------|
| 512M          | FAT 32         | /boot/efi      |
| 80G           | ext4           | /              |
| 50G           | ext4           | /var           |
| 20G           | ext4           | /tmp           |
| 16G           | swap           | swap           |
| Zbytek        | ext4           | /home          |

Erase the entire disk by clicking: *New Partition Table*. 

Giving **/boot** its own partition makes managing multiboot systems easier
because this makes the boot files independent of whatever operating
systems you install or remove. 500MB is more than enough.

Putting **root** in its own partition makes it easy to restore or to nuke
and replace with a different linux. 30GB is more than enough for most
distros, except when you use the *Btrfs* filesystem, then you should
make it 60GB to make room for storing snapshots.

Put home ... page 21.
