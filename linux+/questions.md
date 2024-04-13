# Questions

1.  Which command is used to load a module and its dependencies automatically?

    1. `modprobe`
    2. `lsmod`
    3. `insmod`
    4. `rmmod`

    Answer:

    A.  The `modprobe` command loads the module and its dependencies, if applicable. The `lsmod` command is used to list currently loaded modules, making option B incorrect. The `insmod` command will load a given module but not its dependencies. Option D, `rmmod`, is used to remove a module from memory.
2.  Which option given at boot time within the GRUB2 boot entry configuration will boot the system into single-user mode?

    1. `single-user`
    2. `su`
    3. `single`
    4. `root`

    Answer:

    C.  The keyword `single` given on the Linux kernel command line will boot the system into single-user mode. The other options are not valid.
3.  What is the command to display the default target on a computer running `systemd`?

    1. `systemctl defaults`
    2. `update-rc.d defaults`
    3. `systemctl runlevel`
    4. `systemctl get-default`

    Answer:

    D.  The `systemctl get-default` command will show the default target. The other commands and options are not valid.
4.  Which command is used to obtain a list of USB devices?

    1. `usb-list`
    2. `lsusb`
    3. `ls-usb`
    4. `ls --usb`

    Answer:

    B.  The `lsusb` command is used to obtain a basic list of USB devices on a system. This can be helpful when preparing a USB device with a boot image, such as when you need to boot the system from USB. The other commands are not valid. In the case of option D, the `ls` command is valid, but there is no `--usb` option.
5.  Which command can be used to obtain a list of currently loaded kernel modules?

    1. `insmod`
    2. `modlist`
    3. `ls ––modules`
    4. `lsmod`

    Answer:

    D.  The `lsmod` command is used to list currently loaded kernel modules, thereby making option D correct for this question. The `insmod` command (option A) is used to load modules. Option C is a valid command but not a valid option for that command, and option B does not exist.
6.  When running with a Unified Extensible Firmware Interface (UEFI) system, to which partition will the EFI system partition typically be mounted?

    1. `/etc/efi`
    2. `/efi`
    3. `/sys/efi`
    4. `/boot/efi`

    Answer:

    D.  The ESP is typically mounted at `/boot/efi`.
7.  Assuming that a USB disk contains a single partition and is made available on `/dev/sdb`, which command mounts the disk in `/media/usb`?

    1. `mount /dev/sdb1 /media/usb`
    2. `usbconnect /dev/sdb0 /media/usb`
    3. `mount /dev/sdb0 /media/usb`
    4. `usbmount /dev/sdb1 /media/usb`

    Answer:

    A.  The `mount` command is used to mount drives in Linux. The source and destination mount point are expected as arguments. Drive partitions begin at number 1, making the first partition number 1.
8.  What is one reason a device driver does not appear in the output of `lsmod`, even though the device is loaded and working properly?

    1. The use of `systemd` means drivers are not required for most devices.
    2. The use of an `initrd.img` means support is enabled by default.
    3. The system does not need a driver for the device.
    4. Support for the device has been compiled directly into the kernel.

    Answer:

    D.  If a working device does not appear in `lsmod`, it typically means the kernel has a driver already loaded by virtue of being compiled into the kernel itself rather than loaded through a module. The use of `systemd` (option A) or an `initrd.img` (option B) would have no effect.
9.  Which option to `rmmod` will cause the module to wait until it's no longer in use to unload the module?

    1. `-test`
    2. `-b`
    3. `-w`
    4. `-unload`

    Answer:

    C.  The `-w` option causes the module to wait until it's no longer needed prior to unloading. The other options are not valid for `rmmod`.
10. Which command will output a new GRUB configuration file and send the output to the correct location for booting?

    1. `update-grub`
    2. `update-grub boot > /boot/grub.cfg`
    3. `grub-rc.d`
    4. `grub-boot`

    Answer:

    A.  The `update-grub` is an alias or shortcut for the `grub-mkconfig -o /boot/grub/grub.cfg` command. On some variants of Linux, the `update-grub` command is known as `grub2-update`. The other options are not valid for this purpose. Options C and D are not valid commands, while option B contains invalid options and an invalid location for the destination file.
11. What is the maximum number of primary partitions available on an MBR partitioning system?

    1. Two
    2. Four
    3. One
    4. Five

    Answer:

    B.  MBR-based disks can be partitioned with up to four primary partitions, one of which can be further partitioned or extended into logical partitions.
12. When working with disk partitions through a tool like `fdisk`, you see the type 0x82. Which type of partition is this?

    1. Linux
    2. Linux swap
    3. NTFS
    4. FAT

    Answer:

    B.  0x82 is Linux swap, while 0x83 is Linux. NTFS is 0x07, and FAT is 0.0c.
13. Which file should you edit when using GRUB2 in order to define or set options like the timeout?

    1. `/etc/default/grub`
    2. `/etc/grub/boot`
    3. `/etc/boot/grub.d`
    4. `/grub.d/boot`

    Answer:

    A.  The `/etc/default/grub` file can be used for this purpose. You may also edit `/boot/grub/grub.cfg`, but this was not an option given for this question.
14. Which option for the `grub2-mkconfig` command sends output to a file instead of `STDOUT`?

    1. `-stdout`
    2. `--fileout`
    3. `-o`
    4. `-f`

    Answer:

    C.  The `-o` option can be used to specify a destination file to which output will be sent instead of to `STDOUT`. The other options listed in this question do not exist.
15. Of the following choices, which size would be most appropriate for the `/boot` partition of a Linux system?

    1. At least 1 GB.
    2. Between 100 MB and 200 MB.
    3. `/boot` should not be partitioned separately.
    4. Less than 5 MB.

    Answer:

    A.  The recommended `/boot` partition size has increased and it is now recommended to be at least 1 GB. The used space within `/boot` will increase as more kernels are added, such as during an upgrade process. The size should not be set too small because upgrade processes can fail if the partition becomes full.
16. Which of the following commands initializes a physical disk partition for use with LVM?

    1. `lvmcreate`
    2. `pvcreate`
    3. `vgextend`
    4. `pvs`

    Answer:

    B.  The `pvcreate` command initializes a physical partition for future use as a logical volume with LVM. The `pvs` command displays information about physical volumes but is not used to initialize the physical disk partition. The `vgextend` command is valid but not for the scenario provided. The `lvmcreate` command does not exist.
17. Which of the following commands installs GRUB into the MBR of the second SATA disk?

    1. `grub2-install /dev/hdb2`
    2. `grub2-install /dev/sda2`
    3. `grub2-config /dev/sda`
    4. `grub2-install /dev/sdb`

    Answer:

    D.  The `grub2-install` command is used to install GRUB onto a disk. The second SATA disk would be `/dev/sdb`, therefore making option D the correct answer.
18. Which command is used to create a logical volume with LVM?

    1. `pvcreate`
    2. `lvmcreate`
    3. `lvcreate`
    4. `volcreate`

    Answer:

    C.  The `lvcreate` command is used to create logical volumes with LVM. The `pvcreate` command initializes physical volumes prior to creating logical volumes. The commands in the other two options for this question do not exist.
19. What is the logical order for creation of an LVM logical volume?

    1. Physical volume creation, volume group creation, logical volume creation
    2. Physical volume creation, logical volume creation, volume group creation
    3. Logical volume creation, physical volume creation, volume group creation
    4. LVM creation, format, partition

    Answer:

    A.  Physical volumes are initialized first, followed by volume group creation, and then logical volume creation.
20. Which command should be run after making a change to the `/etc/default/grub` file?

    1. `grub`
    2. `grub-mkconfig`
    3. `grub-inst`
    4. `reboot`

    Answer:

    B.  The `grub-mkconfig` command should be run after making a change to the `/etc/default/grub` file so that a new configuration file can be created with the changed option(s).
21. Which command is used to change details of a logical volume?

    1. `lvmcreate`
    2. `pvcreate`
    3. `lvchange`
    4. `lvmscan`

    Answer:

    C.  The `lvchange` command configures details about a logical volume, including whether that volume appears to be available.
22. A hard drive is reported as `hd(0,0)` by the GRUB Legacy configuration file. To which of the following disks and partitions does this correspond?

    1. `/dev/hdb2`
    2. `/dev/hda0`
    3. `/dev/disk1`
    4. `/dev/sda1`

    Answer:

    D.  GRUB Legacy begins counting at 0 and separates the disk letter and partition with a comma, therefore making `0,0` the first partition on the first disk. Options A and C are not the first disk on the system, and option B contains a nonexistent partition.
23. Which of the following commands installs GRUB into the master boot record (MBR) of the first SATA drive?

    1. `grub-install /dev/hda`
    2. `grub-install /dev/sda`
    3. `grub-install /dev/hd0,0`
    4. `grub -i /dev/hda`

    Answer:

    B.  The command to install GRUB is `grub-install`, and the first SATA drive is `/dev/sda`. A device listed as `hda` is typically a PATA drive, thereby making those options incorrect.
24. Which option given to a `yum` command will install a given package?

    1. `update`
    2. `configure`
    3. `install`
    4. `get`

    Answer:

    C.  The `yum install` command will install a given package. The `update` option will update a package. The other options listed do not exist.
25. After a new hard drive is inserted into the system, what is the correct order to make the drive ready for use within Linux?

    1. Use `fdisk` to create partitions, and then mount the partitions.
    2. Mount the partitions.
    3. Use `fdisk` to create partitions and mount `-a` to mount all the newly created partitions.
    4. Use `fdisk` to create partitions, then format the partitions using a command such as `mkfs`, and then mount the partitions.

    Answer:

    D.  The first step is to use `fdisk` to create one or more partitions. Then format the partitions, and then mount the partitions for use. Various filesystem types can be created with `mkfs` and its subcommands. These filesystem types include `ext3`, `ext4`, `xfs`, and `ntfs`.
26. When working with an `rpm` package file and using `rpm2cpio`, by default the output is sent to which location?

    1. `STDOUT`
    2. The file `cpio.out`
    3. The file `a.out`
    4. The file `/tmp/cpi.out`

    Answer:

    A.  `rpm2cpio` sends its output to `STDOUT` by default, and therefore that output needs to be redirected to a file in most cases.
27. Which of the following describes a primary difference between `ext2` and `ext3` filesystems?

    1. `ext3` was primarily a bug-fix update to `ext2`.
    2. `ext3` includes journaling for the filesystem.
    3. `ext3` completely changed the tools needed for management of the disks.
    4. `ext3` has no significant differences.

    Answer:

    B.  The addition of journaling in `ext3` increased filesystem reliability and performance.
28. According to the Filesystem Hierarchy Standard (FHS), what is the correct location for add-on application software packages?

    1. `/etc`
    2. `/var`
    3. `/tmp`
    4. `/opt`

    Answer:

    D.  The `/opt` hierarchy is used for add-on application software packages. The `/etc` hierarchy is configuration information, while `/var` is also data files but variable files such as mail files. The `/tmp` directory is for temporary files. Because each path begins with a `/`, it is considered an absolute path.
29. Which option to the `mount` command will mount all filesystems that are currently available in `/etc/fstab?`

    1. `-f`
    2. `-d`
    3. `-a`
    4. `-m`

    Answer:

    C.  The `-a` option mounts all filesystems in `/etc/fstab` that are currently available. Of the other options listed, only the `-f` option is available, and it is a shortcut to the “fake” option, which does not do anything except perform a dry run of the mount.
30. Which option of the `systemctl` command will change a service so that it runs on the next boot of the system?

    1. `enable`
    2. `startonboot`
    3. `loadonboot`
    4. `start`

    Answer:

    A.  The `enable` option configures the service to start on boot. The `start` option, option D, is used to start a service immediately. The other options are not valid for this command.
31. Which option to `xfs_metadump` displays a progress indicator?

    1. `-g`
    2. `-p`
    3. `-f`
    4. `-v`

    Answer:

    A.  The `-g` option displays progress of the dump. The other options listed do not exist.
32. The system is running out of disk space within the home directory partition, and quotas have not been enabled. Which command can you use to determine the directories that might contain large files?

    1. `du`
    2. `df`
    3. `ls`
    4. `locate`

    Answer:

    A.  The `du` command will report on disk usage for the specified directory in a recursive manner, unlike the other commands shown here.
33. Which file contains information about the filesystems to mount, their partitions, and the options that should be used to mount them?

    1. `/etc/filesystems`
    2. `/etc/mounts`
    3. `/etc/fstab`
    4. `systemd.mount`

    Answer:

    C.  The `/etc/fstab` file is used to store information about the filesystems to mount within the system. The `systemd.mount` option refers to the configuration files used by `systemd` related to filesystems.
34. According to the FHS, what is the proper mount point for removable media?

    1. `/etc`
    2. `/srv`
    3. `/tmp`
    4. `/media`

    Answer:

    D.  The `/media` mount point is used for removable media. See [`https://refspecs.linuxfoundation.org/FHS_3.0/fhs/index.html`](https://refspecs.linuxfoundation.org/FHS\_3.0/fhs/index.html) for more information on the FHS.
35. How many SCSI devices are supported per bus?

    1. 7 to 15
    2. 2 to 4
    3. 12
    4. 4

    Answer:

    A.  SCSI supports 7 to 15 devices per bus, depending on the type of SCSI. The `lsscsi` command displays device information.
36. Which option to `umount` will cause the command to attempt to remount the filesystem in read-only mode if the unmounting process fails?

    1. `-o`
    2. `-r`
    3. `-f`
    4. `-v`

    Answer:

    B.  The `-r` option causes `umount` to attempt to remount in read-only mode. The `-v` option is verbose mode, and the `-f` option forces the operation. The `-o` option does not exist.
37. Which of the following represents the correct format for the `/etc/fstab` file?

    1. `<directory> <device> <type> <options>`
    2. `<device> <type> <options>`
    3. `<device> <type> <options> <directory> <dump> <fsck>`
    4. `<device> <directory> <type> <options> <dump> <fsck>`

    Answer:

    D.  The proper order is the device (UUID or partition) followed by the directory to mount that device, followed by its type and options, and then the dump and `fsck` settings.
38. Which of the following commands is used to identify the UUID for partitions?

    1. `blkid`
    2. `partprobe`
    3. `find`
    4. `cat`

    Answer:

    A.  The `blkid` command will show partition UUIDs. You can also get this information with the `lsblk -no +UUID <partition>` command. The `partprobe` command is used to update the partition table at the kernel level. The other commands shown in this question do not accomplish the required task.
39. The `xfs_info` command is functionally equivalent to which command and option?

    1. `xfs_test -n`
    2. `xfs_list`
    3. `tunexfs -i`
    4. `xfs_growfs -n`

    Answer:

    D.  The `xfs_info` command is equivalent to `xfs_growfs -n`.
40. Which of the following commands will create a `btrfs` filesystem on the first SATA drive?

    1. `mkfs /dev/sda1`
    2. `mkfs.btrfs /dev/sda`
    3. `mkfs.btr2fs /dev/sda1`
    4. `mkfs –b /dev/sda`

    Answer:

    B.  The `mkfs.btrfs` command is used to create `btrfs` filesystems on block storage and does not require the drive to be partitioned.
41. Which command and option can be used to determine whether a given service is currently loaded?

    1. `systemctl ––ls`
    2. `telinit`
    3. `systemctl status`
    4. `sysctl -a`

    Answer:

    C.  Out of the options given, the `systemctl status` command and option are the most appropriate. The `telinit` and `sysctl` commands are not used for this purpose. Likewise, the `--ls` option is not valid for `systemctl`.
42. Which command can be used to change the partitioning scheme for a disk, such as to change the size of existing partitions without deleting them?

    1. `resize2fs`
    2. `parted`
    3. `mkfs`
    4. `rfdisk`

    Answer:

    B.  The `parted` command can be used to resize partitions in such a way. The `mkfs` command is not used for this purpose, and the other two options do not exist.
43. Which of the following commands will mount a USB device at `/dev/sdb1` into the `/mnt/usb` directory, assuming a VFAT filesystem for the USB drive?

    1. `mount -t vfat /dev/sdb1 /mnt`
    2. `usbmount /dev/sdb1 /mnt/usb`
    3. `mount -t vfat /dev/sdb1 /mnt/usb`
    4. `mount -t usb /dev/sdb1 /mnt/usb`

    Answer:

    C.  The VFAT filesystem is known as `vfat` to the `mount` command, and the other elements of the `mount` command are standard.
44. Which option within `gdisk` will change the partition name?

    1. `n`
    2. `b`
    3. `v`
    4. `c`

    Answer:

    D.  The `c` option in `gdisk` is used to change the partition name. The `n` option creates a new partition, the `v` option verifies the disk, and the `b` option creates a backup of GUID Partition Table (GPT) data to a file.
45. Which command on a `systemd`-controlled system would place the system into single-user mode?

    1. `systemctl stop`
    2. `systemctl isolate rescue.target`
    3. `systemctl single-user`
    4. `systemctl runlevel one`

    Answer:

    B.  The `isolate` option is used to move the system into the target specified, thereby making option B the correct one. The `stop` option stops a service. The other options do not exist.
46. Which options to `fsck` can be used to check all filesystems listed in `/etc/fstab` while excluding the root partition?

    1. `-NR`
    2. `-AR`
    3. `-X`
    4. `-C`

    Answer:

    B.  The `-A` option checks all filesystems in `/etc/fstab`, while the `-R` option excludes the root filesystem.
47. Which option in `/etc/fstab` sets the order in which the device is checked at boot time?

    1. `options`
    2. `dump`
    3. `fsck`
    4. `checkorder`

    Answer:

    C.  The `fsck` option, which is represented as a number in the `/etc/fstab` file, sets the order in which the device is checked at boot time.
48. Which file is used to indicate the local time zone on a Linux server?

    1. `/etc/timez`
    2. `/etc/timezoneconfig`
    3. `/etc/timezone`
    4. `/etc/localtz`

    Answer:

    C.  The file `/etc/timezone` is used to indicate the local time zone. The other files listed as options do not exist.
49. Within which directory will you find files related to the time zone for various regions?

    1. `/etc/timezoneinfo`
    2. `/etc/zoneinfo`
    3. `/var/zoneinfo`
    4. `/usr/share/zoneinfo`

    Answer:

    D.  Within the `/usr/share/zoneinfo` hierarchy, you will find information on the various regions and time zones available. The files within this hierarchy can be symlinked to `/etc/localtime`.
50. Which option best describes the following, gathered with the `ls -la` command?

    `lrwxrwxrwx. 1 root root 35 Jul 8 2014 .fetchmailrc -> .configs/fetchmail/.fetchmailrc`

    1. It is a file called `.fetchmailrc` that is linked using a symbolic link.
    2. It is a file called `.configs/fetchmail/.fetchmailrc` that is owned by `lrwxrwxrwx`.
    3. It is a directory called `.fetchmailrc` that is owned by user Jul.
    4. It is a local directory called `.configs/fetchmail/.fetchmailrc`.

    Answer:

    A.  The listing shows a symbolic linked file created with the `ln` command located in the current directory, linked to `.configs/fetchmail/.fetchmailrc`. The file is owned by the root user and root group and was created on July 8, 2014.
51. Which environment variable controls the format of dates and times, such as a 12-hour or 24-hour formatted clock?

    1. `LOCALE_DATE`
    2. `DATE_FORMAT`
    3. `LC_TIME`
    4. `LC_DATE`

    Answer:

    C.  The `LC_TIME` environment variable is used to control the display and behavior of the date and time and can be changed to a different locale in order to achieve the desired display and behavior of date and time formatting. The other options shown for this question do not exist.
52. Which of the following encodings provides a multibyte representation of characters?

    1. ISO-8859
    2. UTF-8
    3. ISO-L
    4. UFTMulti

    Answer:

    B.  UTF-8 provides multibyte character encoding and is generally accepted as the standard for encoding moving forward. ISO-8859 is single-byte encoded. The other answers are not valid.
53. Which command can be used to view the available time zones on a system?

    1. `tzd`
    2. `/etc/locale`
    3. `timedatectl`
    4. `tzsel`

    Answer:

    C.  The `timedatectl` command includes a `list-timezones` subcommand to show known time zones. The `tzsel` command does not exist, but there is a similar command called `tzselect` that will, by default, display a step-by-step menu to select a time zone. The eventual output will include a region/time-zone line, such as America/Chicago, as output.
54. Which option to `lspci` is used to display both numeric codes and device names?

    1. `-numdev`
    2. `-n`
    3. `-nn`
    4. `-devnum`

    Answer:

    C.  The `-nn` option displays both numbers and device names, thus making option C correct. The `-n` option (option B) displays only numbers. The other two options do not exist.
55. Which of the following values for the `LANG` variable will configure the system to bypass locale translations where possible?

    1. `LANG=COMPAT`
    2. `LANG=NONE`
    3. `LANG=C`
    4. `LANG=END`

    Answer:

    C.  Setting `LANG=C` is an alias for POSIX compatibility and will cause programs to bypass locale translations. The other options shown for `LANG` are not valid.
56. If you need to temporarily reconfigure all locale variables and settings for a given session, which environment variable can be used?

    1. `LC_LIST`
    2. `LC_GLOBAL`
    3. `LC_ALL`
    4. `ALL_LOCALE`

    Answer:

    C.  The `LC_ALL` variable can be used to set environment variables such as the locale and will override others. This can be used when there is a need for a temporary change. The other variables listed here are not used for this purpose and are not created by default.
57. Which of the following commands will set the systemwide time zone to `'America/Los_Angeles'`?

    1. `ln -sf /usr/share/zoneinfo/America/Los_Angeles /etc/localtime`
    2. `ln -sf America/Los_Angeles ; /etc/localtime`
    3. `ln -sd /etc/localtime /usr/share/timezone/America/Los_Angeles`
    4. `ln -sf /etc/localtime /usr/share/zoneinfo/America/Los_Angeles`

    Answer:

    A.  The `ln` command is used for this purpose, and the `-s` option creates a symbolic or soft link, while `-f` forces or overwrites the destination. The other options and order of commands are not valid.
58. Which locale-related variable is used for currency-related localization?

    1. `LC_MONE`
    2. `LC_CURRENCY`
    3. `LC_MONETARY`
    4. `LC_CURR`

    Answer:

    C.  The `LC_MONETARY` variable is used by certain programs to determine the localization for currency.
59. Which command is used to query and work with the hardware clock on the system?

    1. `hwc`
    2. `ntpdate`
    3. `systime`
    4. `hwclock`

    Answer:

    D.  The `hwclock` command is used to both query and set the hardware clock, such as the one maintained by the system firmware or Basic Input/Output System (BIOS). The `ntpdate` command is used to set the local system time but is not related to the hardware clock. The other commands are not valid.
60. Which option to the `date` command can be used to set the date and time?

    1. `date -f`
    2. `date -t`
    3. `date --change`
    4. `date -s`

    Answer:

    D.  The `-s` option sets the date and time as specified within the command. If there is another means to automatically set the date, it may override the change. For example, if `ntpd` or `chrony` is running, one of those processes may alter the date even after it has been set with `date -s`.
61. Which function of the `hwclock` command will set the hardware or BIOS clock to the current system time?

    1. `-w`
    2. `-s`
    3. `-a`
    4. `-m`

    Answer:

    A.  The `-w` option sets the hardware clock to the current system time. The `-s` option does the opposite, setting the system time to the hardware clock. There is no `-a` or `-m` function for `hwclock`.
62. Which of the following commands sets the hardware or BIOS clock to UTC based on the current system time?

    1. `hwclock --systohc --utc`
    2. `hwclock --systohc --localtime`
    3. `hwclock --systohc`
    4. `hwclock --systoutc`

    Answer:

    A.  `--systohc` will set the hardware clock according to the current system time. The use of `--utc` is required in order to ensure that the time is set to UTC. If `--utc` is omitted, the time will default to whatever was used last time the command was run, which could be UTC but might be local time instead. Therefore, the best option is A.
63. Which of the following commands shows the current default route without performing DNS lookups on the IP address(es) involved?

    1. `netstat -rn`
    2. `netstat -n`
    3. `netstat -r`
    4. `netstat -f`

    Answer:

    A.  The `netstat` command can be used for this purpose, and the `-r` option displays the current routes. The addition of `-n` prevents DNS lookups, which can help with performance.
64. A Serial ATA (SATA) disk will use which of the following identifiers?

    1. `/dev/hdX`
    2. `/dev/sataX`
    3. `/dev/sdX`
    4. `/disk/sataX`

    Answer:

    C.  SATA disks are addressed as `/dev/sdX`, just like a SCSI disk. `/dev/hdX` is a traditional ATA disk. The other options do not exist.
65. Which of the following commands adds a default gateway of 192.168.1.1 for interface `eth0`?

    1. `route add default gateway 192.168.1.1 eth0`
    2. `eth0 --dg 192.168.1.1`
    3. `route add default gw 192.168.1.1 eth0`
    4. `route define eth0 192.168.1.1`

    Answer:

    C.  The `route` command is used for this purpose, and adding a route is done with the `add` option. The default gateway is added using the `default gw` keywords followed by the IP address of the gateway and the adapter.
66. Which option for the `host` command will query for the authoritative name servers for a given domain?

    1. `-t ns`
    2. `-t all`
    3. `-ns`
    4. `-named`

    Answer:

    A.  The `host` command enables changing of the query type with the `-t` option. Using `ns` as the type will query for the name servers for a given domain. There is no `all` type, and the other options are also invalid.
67. Which option for the `ping` command enables you to choose the interface from which the ICMP packets will be generated?

    1. `-i`
    2. `-I`
    3. `-t`
    4. `-a`

    Answer:

    B.  The `-I` option enables the choice of interface. A lowercase `-i` option sets the interval, while `-a` indicates an audible ping. Finally, `-t` enables a TTL-based ping only.
68. Which of the following commands queries for the mail servers for the domain [`example.com`](http://example.com/)?

    1. `dig` [`example.com`](http://example.com/) `mx`
    2. `dig` [`example.com`](http://example.com/)
    3. `host -t smtp` [`example.com`](http://example.com/)
    4. `dig` [`example.com`](http://example.com/) `smtp`

    Answer:

    A.  The `host` or `dig` command can be used for this purpose by setting the type to `mx`. The `mx` type will query for the mail exchanger for the given domain. There is no `smtp` type.
69. Which of the following addresses represents the localhost in IPv6, such as you might find in `/etc/hosts`?

    1. `0:1`
    2. `::1`
    3. `127:0:1`
    4. `:127:0:0:1`

    Answer:

    B.  The localhost address for IPv6 can be written as `::1`. Addresses shown like `127` represent the IPv4 localhost range but are not written properly for IPv4 or IPv6.
70. Which command can be used to listen for netlink messages on a network?

    1. `ip monitor`
    2. `netlink -a`
    3. `ip netlink`
    4. `route`

    Answer:

    A.  The `ip` command with the `monitor` option/subcommand will display netlink messages as they arrive. There is no `netlink` subcommand for `ip`, and the `route` command will not work for this purpose.
71. Which of the following configuration lines in `/etc/nsswitch.conf` causes a lookup for group information to first use local files and then use LDAP?

    1. `group: files ldap`
    2. `lookup: group [local ldap]`
    3. `group: [local ldap]`
    4. `group: localfiles ldap`

    Answer:

    A.  The syntax is `database: <databasename>` with additional database names separated by spaces, as shown in the correct option for this question.
72. Which of the following `dig` commands sends the query for [`example.com`](http://example.com/) directly to the server at 192.168.2.5 rather than to a locally configured resolver?

    1. `dig` [`example.com`](http://example.com/) `@192.168.2.5`
    2. `dig -t 192.168.2.5` [`example.com`](http://example.com/)
    3. `dig -s 192.168.2.5` [`example.com`](http://example.com/)
    4. `dig server=192.168.2.5` [`example.com`](http://example.com/)

    Answer:

    A.  The `@` symbol is used to indicate a server to which the query will be sent directly. This can be quite useful for troubleshooting resolution problems by sending the query directly to an authoritative name server for the domain. Of the other options, `-t` sets the type, and the other options are not valid.
73. Which of the following commands will enumerate the `hosts` database?

    1. `getent hosts`
    2. `gethosts`
    3. `nslookup`
    4. `host`

    Answer:

    A.  The `getent` command is used for working with NSS databases, and `getent hosts` will display the available hosts using the databases configured in `/etc/nsswitch.conf`.
74. Which of the following configuration lines will set the DNS server to 192.168.1.4 using `/etc/resolv.conf`?

    1. `dns 192.168.1.4`
    2. `dns-server 192.168.1.4`
    3. `nameserver 192.168.1.4`
    4. `name-server 192.168.1.4`

    Answer:

    C.  The configuration option is `nameserver`, and the value for the option is the IP address of the desired name server. Several options affect how name resolution is performed, such as the number of attempts and timeout. See `resolv.conf(5)` for more information.
75. Which of the following commands adds a route to the server for the network 192.168.51.0/24 through its gateway 192.168.22.1?

    1. `route add -net 192.168.51.0 netmask 255.255.255.0 gw 192.168.22.1`
    2. `route add -net 192.168.51/24 gw 192.168.22.51`
    3. `route -net 192.168.51.0/24 192.168.22.1`
    4. `route add 192.168.51.1 -n 192.168.22.0//255.255.255.0`

    Answer:

    A.  The `route` command can be used for this purpose, and the syntax includes the network range, denoted with the `-net` option, followed by the word `netmask` and the masked bits, followed by the letters `gw` and the IP address of the gateway. The other options shown are invalid for a variety of reasons, including missing keywords and options and order.
76. Which of the following commands shows network services or sockets that are currently listening along with sockets that are not listening?

    1. `netstat -a`
    2. `netlink -a`
    3. `sockets -f`
    4. `opensock -l`

    Answer:

    A.  The `netstat` command is used for this purpose, and the `-a` option displays all sockets, listening and non-listening. Note that it's frequently helpful to add the `-n` option, or combine options as in `netstat –an`, in order to prevent name lookup. Doing so can significantly improve performance of the command.
77. When partitioning a disk for a mail server running Postfix, which partition/mounted directory should be the largest in order to allow for mail storage?

    1. `/etc`
    2. `/usr/bin`
    3. `/mail`
    4. `/var`

    Answer:

    D.  The partition containing `/var` should be the largest for a mail server because mail spools are stored within this hierarchy. The `/etc/` hierarchy is usually small, as is `/usr/bin`. The `/mail` directory does not exist by default.
78. Which of the following commands will change the default gateway to 192.168.1.1 using `eth0`?

    1. `ip route default gw 192.168.1.1`
    2. `ip route change default via 192.168.1.1 dev eth0`
    3. `ip route default gw update 192.168.1.1`
    4. `ip route update default 192.168.1.1 eth0`

    Answer:

    B.  The `ip route` command can be used for this purpose, and its syntax uses a `change` command and the `via` keyword. The same operation could be completed with the `route` command but would require deleting the existing gateway first and then re-adding a new default gateway.
79. Which of the following commands displays the Start of Authority information for the domain [`example.com`](http://example.com/)?

    1. `dig` [`example.com`](http://example.com/) `soa`
    2. `dig` [`example.com`](http://example.com/) `authority`
    3. `dig` [`example.com`](http://example.com/) `-auth`
    4. `dig -t auth` [`example.com`](http://example.com/)

    Answer:

    A.  The `soa` type is used to query for Start of Authority records for a domain. Note that in many cases, `dig` will attempt to look up the domain within a given command and may not appear to have had an error. For example, when running option D (`dig -t auth` [`example.com`](http://example.com/)), you will receive information about [`example.com`](http://example.com/), and there will be a line in the output saying that `dig` has ignored the invalid type of `auth`.
80. Assume that you want to enable local client services to go to hosts on the network without needing to fully qualify the name by adding the domain for either [`example.com`](http://example.com/) or [`example.org`](http://example.org/). Which option in `/etc/resolv.conf` will provide this functionality?

    1. `search`
    2. `domain`
    3. `local-domain`
    4. `local-order`

    Answer:

    A.  The `search` option is used for this purpose and can be provided with multiple domain names, each separated by a space or tab. The `domain` option is valid within `/etc/resolv.conf` but does not allow for multiple domain names.
81. Which of the following commands prevents traffic from reaching the host 192.168.1.3?

    1. `route add -host 192.168.1.3 reject`
    2. `route -nullroute 192.168.1.3`
    3. `route add -null 192.168.1.3`
    4. `route add -block 192.168.1.3`

    Answer:

    A.  The `route` command can be used for this purpose, and in the scenario described, a `reject` destination is used for the route. The other options shown are invalid because they use invalid options to the `route` command.
82. Which of the following commands will emulate the `ping` command in Microsoft Windows, where the ping is sent for four packets and then the command exits?

    1. `ping -n 4`
    2. `ping -t 4`
    3. `ping -p 4`
    4. `ping -c 4`

    Answer:

    D.  The `-c` option provides the count of the number of pings to send. The `-n` option specifies numeric output only, while `-p` specifies the pattern to use for the packet content. Finally, the `-t` option sets the TTL.
83. You need to prevent local clients from going to a certain host, `www.example.com`, and instead redirect them to localhost. Which of the following is a method to override DNS lookups for the specified host?

    1. Add a firewall entry for the IP address of `www.example.com` to prevent traffic from passing through it.
    2. Delete `www.example.com` from the route table using the `route` command.
    3. Add a null route to prevent access to the IP address for `www.example.com`.
    4. Add an entry for `www.example.com` in `/etc/hosts` to point to 127.0.0.1.

    Answer:

    D.  The best option for this question is to add an entry for the host in `/etc/hosts`. Doing so will always cause DNS queries to resolve to 127.0.0.1. The other options are not as robust because they rely on `www.example.com` always having the same IP address, or the solutions require additional maintenance to constantly add new IP addresses if `www.example.com`'s IP address changes.
84. Which of the following commands should be executed after running `ip route change`?

    1. `ip route flush cache`
    2. `ip route reload`
    3. `ip route cache reload`
    4. `ip route restart`

    Answer:

    A.  The `ip route flush cache` command should be executed after changing the routes. The other commands shown for this question are not valid.
85. Which option should be used to send a DNS query for an SPF record with `dig`?

    1. `-t txt`
    2. `-t spf`
    3. `-t mx`
    4. `-t mailspf`

    Answer:

    A.  SPF records are stored in the `txt` record type in DNS, thereby making `-t txt` the correct option for this. Of the other answers, only `-t mx` is valid; it returns the mail exchangers for the given domain.
86. When you're viewing the available routes using the `route` command, one route contains flags `UG` while the others contain `U`. What does the letter `G` signify in the route table?

    1. The `G` signifies that the route is good.
    2. The `G` signifies that the route is unavailable.
    3. The `G` signifies that this is a gateway.
    4. The `G` signifies that the route is an aggregate.

    Answer:

    C.  The `G` signifies a gateway within the route table.
87. Which of the following commands requests a zone transfer of [`example.org`](http://example.org/) from the server at 192.168.1.4?

    1. `dig` [`example.org`](http://example.org/) `@192.168.1.4 axfr`
    2. `dig` [`example.org`](http://example.org/) `@192.168.1.4`
    3. `dig` [`example.org`](http://example.org/) `@192.168.1.4 xfer`
    4. `dig` [`example.org`](http://example.org/) `#192.168.1.4 xfer`

    Answer:

    A.  The `axfr` type is a zone transfer, and the `@` symbol signifies the server to which the query will be sent. There is no `xfer` type, and option B is just a normal query for the domain sent to the specified server.
88. Which `yum` option displays the dependencies for the package specified?

    1. `list`
    2. `deplist`
    3. `dependencies`
    4. `listdeps`

    Answer:

    B.  The `deplist` option displays the dependencies for the given package. The `list` option displays information about a specific package, while the other two options are not valid.
89. Which of the following commands can be used to display the current disk utilization?

    1. `df`
    2. `du`
    3. `diskutil`
    4. `diskuse`

    Answer:

    A.  The `df` command displays information on disk usage and can help with planning disk utilization over time. For example, if you note that disk utilization is increasing significantly, preparations can be made to bring more disks online or even to change the log rotation schedule such that logs are rotated faster, thereby freeing up space.
90. You are working with a legacy CentOS 5 system and need to re-create the initial RAM disk. Which of the following commands is used for this purpose?

    1. `mkinitrd`
    2. `mkramdisk`
    3. `mkdisk --init`
    4. `mkfs.init`

    Answer:

    A.  The `mkinitrd` command is used on older systems to create the initial RAM disk. The initial RAM disk is used to load (some might say preload) essential modules for things like disks and other vital components needed for booting.
91. Which of the following commands is used to display the currently loaded modules on a running system?

    1. `ls -mod`
    2. `lsmod`
    3. `tree`
    4. `mod --list`

    Answer:

    B.  The `lsmod` command is used to display currently loaded modules. This is useful for scenarios where you are migrating from the stock or distribution-provided kernel to a custom kernel and need to know which modules to compile into the new kernel. Of the other commands, the `tree` command is valid but not for the scenario provided.
92. Which of the following commands creates a list of modules and their dependencies?

    1. `lsmod`
    2. `depmod`
    3. `modlist`
    4. `listmod`

    Answer:

    B.  The `depmod` command is used to create a list of modules. The list is kept in a file called `modules.dep`, the location of which is dependent on the distribution of Linux in use.
93. Which option to `sysctl` displays all values and their current settings?

    1. `-a`
    2. `-b`
    3. `-d`
    4. `-c`

    Answer:

    A.  The `-a` option displays all values and their current settings for `sysctl`. The `-b` option is binary and displays values without any newlines. The `-d` option is an alias for `-h`, which is help display. There is no `-c` option. The `sysctl` options can also be found in `/etc/sysctl.conf`.
94. Which of the following commands installs a kernel module, including dependencies?

    1. `lsmod`
    2. `modprobe`
    3. `modinst`
    4. `instmod`

    Answer:

    B.  The `modprobe` command examines dependencies for a given module and loads both the dependencies and the requested module.
95. Which command is used to determine the modules on which another module depends?

    1. `modinfo`
    2. `modlist`
    3. `modprobe`
    4. `tracemod`

    Answer:

    A.  The `modinfo` command provides information on a given kernel module. You can use `modinfo` to find out the parameters needed for a given module and the modules on which it depends, among other information. The `modprobe` command is used to load a module. There is no `tracemod` or `modlist` command.
96. Which of the following commands inserts a module into the running kernel but does not resolve dependencies?

    1. `lsmod`
    2. `modinstall`
    3. `insmod`
    4. `moduleinst`

    Answer:

    C.  The `insmod` command inserts a module into the running kernel. It does not, however, attempt to resolve dependencies but rather outputs an error if there are dependent modules or kernel symbols that are not available.
97. Which option to `modprobe` will remove a module and attempt to remove any unused modules on which it depends?

    1. `-v`
    2. `-r`
    3. `-d`
    4. `-f`

    Answer:

    B.  The `-r` option removes the named kernel modules and attempts to remove any modules on which the named module depends, where possible. The `-d` option sets the root directory for modules, while `-v` is verbose and `-f` forces the module to load.
98. Within which of the following directories will you find blacklist information for modules loaded with `modprobe`?

    1. `/etc/blacklist`
    2. `/etc/modprobe.d`
    3. `/etc/blacklist.mod`
    4. `/etc/modprobe`

    Answer:

    B.  The `/etc/modprobe.d` directory is used for storing configuration information related to modules such as that used for blacklisting purposes and also for other configuration information such as `udev` and module options.
99. When working with a CentOS 6 system, which command is used to create the initial RAM disk?

    1. `mkinit`
    2. `dracut`
    3. `mkraminit`
    4. `mkinitfs`

    Answer:

    B.  The `dracut` command is used to create the initial RAM disk for newer systems and has replaced the legacy `mkinitrd` command used for the same purpose.
100.    If you'd like a value set with the `sysctl` command to take effect on boot, within which file should you place the variable and its value?

        1. `/etc/sysctl.cfg`
        2. `/etc/sysctl.conf`
        3. `/lib/sysctl`
        4. `/var/sysctl.conf`

        Answer:

        B.  Variables and values placed in `/etc/sysctl.conf` will take effect on boot. The other files listed are not valid.
101.    Which of the following options to `modprobe` will show the dependencies for a module?

        1. `--show-deps`
        2. `--show-depends`
        3. `--deps`
        4. `--list-depends`

        Answer:

        B.  The `--show-depends` option displays the dependencies for a given module. The other options are not valid for the `modprobe` command.
102.    Which options for the `rpm` command will display verbose output for an installation along with progress of the installation?

        1. `-ivh`
        2. `-wvh`
        3. `––avh`
        4. `––ins-verbose`

        Answer:

        A.  The `-ivh` options will install a file using `rpm`, displaying both verbose output and hash marks for progress. The other options presented do not exist or do not accomplish the specified task.
103.    When working with UEFI, which of the following commands changes the boot order for the next boot?

        1. `efibootmgr -c`
        2. `efibootmgr -b -B`
        3. `efibootmgr -o`
        4. `efibootmgr -n`

        Answer:

        D.  The `-n` option changes the boot order for the next boot only and boots from the specified partition. The `-b` along with `-B` modifies and then deletes the option. The `-o` option sets the boot order. The `-c` option creates a boot number.
104.    Which bootloader can be used to boot from ISO with ISO9660 CD-ROMs?

        1. ISOLINUX
        2. EFIBOOT
        3. ISOFS
        4. BOOTISO

        Answer:

        A.  ISOLINUX provides a means by which CD-ROMs formatted as ISO 9660 can be booted. It's very common to have live CDs or rescue/recovery CDs that use ISOLINUX for boot. The other bootloaders are not valid for this purpose or don't exist.
105.    When using UEFI, which of the following files can be used as a bootloader?

        1. `shim.uefi`
        2. `shim.efi`
        3. `shim.fx`
        4. `efi.shim`

        Answer:

        B.  Due to the decidedly insecure decisions made with the design of Microsoft's UEFI, a shim is often needed to enable Linux to boot on a system with UEFI. The file `shim.efi` can be used as an initial bootloader for this purpose.
106.    Which of the following commands, executed from within the UEFI shell, controls the boot configuration?

        1. `bootcfg`
        2. `bcfg`
        3. `grub-install`
        4. `grcfg`

        Answer:

        B.  The `bcfg` command within the UEFI shell is used to configure bootloaders on a UEFI-based system. The command can accept various parameters to configure how the bootloader and kernel will load on boot. Of the other commands shown, `grub-install` is valid but not within the UEFI shell.
107.    Which of the following can be identified as an initial sector on a disk that stores information about the disk partitioning and operating system location?

        1. Minimal boot record (MBR)
        2. Master boot record (MBR)
        3. Init sector
        4. Master partition table (MPT)

        Answer:

        B.  The master boot record, or MBR, is the first sector on a disk and contains information about the structure of the disk. If the MBR becomes corrupt, all data on the disk may be lost. The other options shown for this question are not valid.
108.    When using PXE boot, which file must exist within `/tftpboot` on the TFTP server for the system that will use PXELINUX for its bootloader?

        1. `pxelinux.tftp`
        2. `pxelinux.boot`
        3. `pxelinux.conf`
        4. `pxelinux.0`

        Answer:

        D.  The file `pxelinux.0` must exist within `/tftpboot` on the TFTP server in order for a system to use PXELINUX for booting. The other files are not valid or necessary for PXELINUX. Once booted, PXE boot can boot using an NFS-mounted filesystem where the filesystem is physically hosted on a different computer.
109.    Which option to `grub-install` will place the GRUB images into an alternate directory?

        1. `--boot-dir`
        2. `-b`
        3. `-boot`
        4. `--boot-directory`

        Answer:

        D.  The `--boot-directory` option enables you to specify an alternate location for GRUB images rather than the default `/boot`. The other options shown for this question are not valid.
110.    When using a shim for booting a UEFI-based system, which of the following files is loaded after `shim.efi`?

        1. `grubx64.cfg`
        2. `grub.conf`
        3. `grubx64.efi`
        4. `efi.boot`

        Answer:

        C.  The `shim.efi` bootloader loads another bootloader, which is `grubx64.efi` by default. The other options are not valid filenames for the purpose described.
111.    Part of the EXT tools, which option to the `mke2fs` command sets the type of filesystem to be created?

        1. `-f`
        2. `-a`
        3. `-t`
        4. `-e`

        Answer:

        C.  The `-t` option sets the filesystem type as `ext2`, `ext3`, or `ext4`. The `mke2fs` command is typically symlinked from `/sbin/mkfs.ext2`, `/sbin/mkfs.ext3`, and `/sbin/mkfs.ext4`. The `-f` option forces `mke2fs` to create a filesystem. The `-a` and `-e` options do not exist.
112.    Which file is used to store a list of encrypted devices that are to be mounted at boot?

        1. `/etc/cryptdev`
        2. `/etc/crypttab`
        3. `/etc/encrtab`
        4. `/etc/fsencrypt`

        Answer:

        B.  The `/etc/crypttab` file contains the filesystems and devices that are encrypted such as those with Linux Unified Key Setup (LUKS). The other file locations do not exist by default and are not related to this question.
113.    Which command will search for a package named `zsh` on a Debian system?

        1. `apt-cache search zsh`
        2. `apt-get search zsh`
        3. `apt-cache locate zsh`
        4. `apt-search zsh`

        Answer:

        A.  The `apt-cache` command is used to work with the package cache, and the `search` option is used to search the cache for the supplied argument, in this case `zsh`. The `apt-get` command is used to work with packages themselves, while the `apt-search` command does not exist. The `apt.conf` file, found either in `/etc/apt/` or `/etc/`, contains several options for how `apt` behaves.
114.    Within which directory will you find the repositories used by `yum`?

        1. `/etc/yum.conf`
        2. `/etc/repos`
        3. `/etc/yum.conf.d`
        4. `/etc/yum.repos.d`

        Answer:

        D.  Configuration files related to the repositories for `yum` are located in `/etc/yum.repos.d`. Of the other options, `/etc/yum.conf` is a file and not a directory, and the other directories do not exist.
115.    You are performing an `xfsrestore`. The `xfsdump` was executed with a block size of 4M. Which option do you need to invoke on `xfsrestore` in order for it to successfully use this dump?

        1. `-b 4M`
        2. `-g 1M`
        3. `-i 1M`
        4. `-k 1028K`

        Answer:

        A.  The block size for import or restore must match the block size used on export or dump. Block size is specified with the `-b` option, thus making option A correct. The other options are not valid for `xfsrestore`.
116.    You see the word `defaults` within `/etc/fstab`. Which options are encompassed within the defaults?

        1. `ro`, `exec`, `auto`
        2. `rw`, `suid`, `dev`, `exec`, `auto`, `nouser`, `async`
        3. `rw`, `exec`, `auto`, `nouser`, `async`
        4. `rw`, `exec`, `nouser`, `async`, `noauto`, `suid`

        Answer:

        B.  A filesystem with the word `defaults` for its mount options will be mounted read-write (`rw`), `suid`, with the ability to have executables (`exec`). The filesystem will be auto-mounted (`auto`), but users will not be able to mount it (`nouser`). Character and block special devices will be interpreted (`dev`), and operations on the disk will be performed in an asynchronous manner (`async`).
117.    Which of the following options to `xfsdump` sets the maximum size for files to be included in the dump?

        1. `-p`
        2. `-s`
        3. `-z`
        4. `-b`

        Answer:

        C.  The `-z` option sets the maximum size for files to be included in the dump. The `-b` option sets the block size but is not related to what is being asked for in this scenario. The `-s` option sets the path for inclusion in the dump, and `-p` sets the interval for progress indicators.
118.    Which partition type is used to indicate a software RAID array, such as an array built with `mdadm`?

        1. 0xmd
        2. \-x-
        3. 0xRD
        4. 0xFD

        Answer:

        D.  A partition type of 0xFD is used for software RAID arrays. This can be set or viewed using a tool such as `fdisk`. The other options shown are not valid partition types.
119.    When working with World Wide Identifiers (WWIDs), within which directory on a Red Hat server will you find symlinks to the current `/dev/sd` device names?

        1. `/dev/disk/wwid`
        2. `/dev/wwid`
        3. `/dev/disk/by-id`
        4. `/dev/sd.wwid`

        Answer:

        C.  The `/dev/disk/by-id` directory contains symbolic links to `/dev/sd`, such as `/dev/sda`. Because WWIDs can be used to identify a device across systems, they are often used within the context of SANs. The other directories listed as options do not exist.
120.    Which of the following commands displays information about a given physical volume in an LVM setup?

        1. `pvdisp`
        2. `pvlist`
        3. `pvdisplay`
        4. `pvl`

        Answer:

        C.  The `pvdisplay` command shows information about a given physical volume. You can use `pvdisplay` to view the device on which the PV is built along with the extent size of the PV. The other commands shown are not valid.
121.    When viewing information in `/dev/disk/by-path` using the command `ls -l`, which of the following filenames represents a LUN from Fibre Channel?

        1. `/dev/fc0`
        2. `pci-0000:1a:00.0-fc-0x500601653ee0025f:0x0000000000000000`
        3. `pci-0000:1a:00.0-scsi-0x500601653ee0025f:0x0000000000000000`
        4. `/dev/fibre0`

        Answer:

        B.  Logical unit numbers (LUNs) that contain the characters `fc` are those found through Fibre Channel. Therein lies the difference between options B and C, where option C contains the letters `scsi`, which would usually represent a local disk. The other options are not valid.
122.    Which of the following commands displays path information for LUNs?

        1. `luninfo -a`
        2. `ls -lun`
        3. `multipath -l`
        4. `dm-multi`

        Answer:

        C.  The `multipath` command is used for administration of devices such as LUNs and can be used for finding the path to LUNs for a server, such as in a SAN configuration. Related, the `multipathd` daemon checks for paths that have failed. The other commands are not valid, with the exception of `ls`: it is valid, but the option shown is not related to LUNs but rather is a combination of various flags to the `ls` command.
123.    Which command is used to remove unused filesystem blocks from thinly provisioned storage?

        1. `thintrim`
        2. `thtrim`
        3. `fstrim`
        4. `fsclean`

        Answer:

        C.  The `fstrim` command is used to remove blocks that are not in use. The `fstrim` command is frequently used in a SAN configuration to give back unused storage to the SAN. The `fstrim` command can also be used with solid-state drives for the same purpose. The other commands shown are not valid.
124.    When using `tune2fs` to set an extended option such as `stripe_width`, which command-line option is needed to signify that an extended option follows?

        1. `-extend`
        2. `-E`
        3. `-e`
        4. `-f`

        Answer:

        B.  The `-E` option signals that an extended option follows, such as `stripe_width`. The `-f` option forces an operation but should not be necessary for this solution, and the `-e` option sets the behavior on error. There is no `-extend` option.
125.    Which option to `mdadm` is used to create a new array?

        1. `--create`
        2. `--start`
        3. `--begin`
        4. `--construct`

        Answer:

        A.  The `--create` option enables creation of a RAID array that will use `md`. The typical argument is the `/dev/mdN` device along with the level. The other options listed are not valid for `mdadm`.
126.    Information about logical volumes can be found in which of the following directories?

        1. `/dev/lvinfo`
        2. `/dev/map`
        3. `/dev/mapper`
        4. `/dev/lvmap`

        Answer:

        C.  The `/dev/mapper` directory contains information about multipath devices such as logical volumes. The other directories are not valid.
127.    Which option to `mdadm` watches a RAID array for anomalies?

        1. `--mon`
        2. `--watch`
        3. `--monitor`
        4. `--examine`

        Answer:

        C.  The `--monitor` option is used to actively watch an array for issues such as disk failure. The monitoring can be done as a daemon and run in the background, thereby alerting when there is an issue.
128.    When running `mdadm` in monitor mode, which option within `/etc/mdadm.conf` sets the destination for email if an issue is discovered?

        1. `MAILTO`
        2. `MAILADDR`
        3. `MAILFROM`
        4. `MAILDEST`

        Answer:

        B.  The `MAILADDR` option sets the destination address for mail about RAID events that are noted by `mdadm` when in monitor mode.
129.    When using the `ip` command, which protocol family is used as the default if not otherwise specified?

        1. `tcpip`
        2. `ip`
        3. `inet`
        4. `arp`

        Answer:

        C.  The `ip` command defaults to the `inet` family if not otherwise specified with the `-f` option. The command will attempt to guess the correct family and fall back to `inet`. The other families listed as options for this command are not valid for use with the `ip` command.
130.    Which command is used for setting parameters such as the essid, channel, and other related options for a wireless device?

        1. `ifconfig`
        2. `iwconfig`
        3. `wlancfg`
        4. `ifcfg`

        Answer:

        B.  The `iwconfig` command, which is similar to the `ifconfig` command, works with an individual wireless interface to set and display parameters. Of the other commands, the `ifconfig` command is valid but not used for wireless, and `ifcfg` is intended as a replacement for `ifconfig`. The other commands are not valid.
131.    Which of the following commands shows network sockets and their allocated memory?

        1. `ss -m`
        2. `mpas`
        3. `mem`
        4. `free`

        Answer:

        A.  The `ss` command provides many of the same functions as `netstat` but can show some extended information, such as memory allocation for a given socket. The `free` command shows memory usage but not by socket, and the other two commands do not exist.
132.    Which option to the `ss` command shows the process IDs associated with the socket?

        1. `-l`
        2. `-a`
        3. `-p`
        4. `-f`

        Answer:

        C.  The `-p` option shows the process IDs associated with a given socket within the `ss` output. The `-a` option is all sockets, while `-l` is listening sockets. The `-f` option is used to specify the protocol family.
133.    On a Debian system, within which directory hierarchy will you find configuration information and directories to hold scripts to be run when an interface is brought up or taken down?

        1. `/etc/netconf`
        2. `/etc/netconfig`
        3. `/etc/net.conf.d`
        4. `/etc/network`

        Answer:

        D.  The `/etc/network` directory contains information on network interfaces and contains directories that then further contain scripts to be executed when interfaces are brought up or down. The other directories listed do not exist.
134.    Which of the following characters are valid for hostnames in `/etc/hosts`?

        1. Alphanumerics, minus, underscore, and dot
        2. Alphanumerics, minus, and dot
        3. Alphanumerics and dot
        4. Alphanumerics

        Answer:

        B.  Only alphanumerics, minus sign or dash, and dot are valid for hosts in `/etc/hosts`.
135.    Which of the following configuration lines in `/etc/resolv.conf` enables debugging?

        1. `debug`
        2. `options debug`
        3. `option debug`
        4. `enable-debug`

        Answer:

        B.  Options within `/etc/resolv.conf` are preceded with the `options` keyword followed by one or more options such as `debug`.
136.    The system contains an NFS mounted filesystem that has become unreachable. Which option should be passed to `umount` in order to force the unmounting of the filesystem?

        1. `-nfs`
        2. `--fake`
        3. `-f`
        4. `-n`

        Answer:

        C.  The `-f` option will force the `umount` to occur. The `--fake` option is essentially a dry run in that it won't actually unmount a filesystem. The other two options do not exist.
137.    Which of the following commands will send the output of the `grub2-mkconfig` command to the correct location for booting?

        1. `grub2-mkconfig --output=/boot/grub2/grub.cfg`
        2. `grub2-mkconfig --file=/boot/grub2.menu`
        3. `grub2-mkconfig --file=/boot/grub.lst`
        4. `grub2-mkconfig --output=/boot/menu.lst`

        Answer:

        A.  The `--output` option configures the location for output of the command instead of `STDOUT`.
138.    Which PXE Linux binary file is required for booting from HTTP or FTP?

        1. `lpxelinux.0`
        2. `pxelinux.http`
        3. `netpxlinux.0`
        4. `netpxe.0`

        Answer:

        A.  The file `lpxelinux.0` contains the necessary code to support booting from HTTP and FTP.
139.    The file `/etc/grub2.cfg` is typically a symbolic link to which file?

        1. `/boot/grub.conf`
        2. `/boot/grub2/grub.cfg`
        3. `/boot/grub2.conf`
        4. `/etc/sysconfig/grub2.cfg`

        Answer:

        B.  The file `/etc/grub2.cfg` is usually a symbolic link to `/boot/grub2/grub.cfg`.
140.    Which of the following describes a difference between `vmlinuz` and `vmlinux`?

        1. `vmlinuz` is used for zOS systems, and `vmlinux` is used for x86 architecture.
        2. `vmlinuz` is used for 64-bit systems, and `vmlinux` is used for 32-bit systems.
        3. `vmlinuz` is compressed, whereas `vmlinux` is not.
        4. `vmlinuz` contains additional binary code for certain systems.

        Answer:

        C.  The `vmlinuz` file has been compressed and therefore consumes less disk space than `vmlinux`. Both contain the Linux kernel in binary format.
141.    Which of the following is the location in which kernel modules are stored?

        1. `/usr/modules`
        2. `/modules`
        3. `/usr/lib/modules/{kernel-version}`
        4. `/usr/modules/{kernel-version}`

        Answer:

        C.  Modules are stored in `/usr/lib/modules/{kernel-version}`.
142.    Which `rpm` option can be used to verify that no files have been altered since installation?

        1. `-V`
        2. `-v`
        3. `––verbose`
        4. `––filesum`

        Answer:

        A.  The `-V` or, `--verify`, option will check the files in a given package against versions (or checksums) in the package database. If no files have been altered, then no output is produced. Note that output may be produced for files that are changed during installation or for other reasons. Note also the use of an uppercase `V` for this option, as opposed to the lowercase `v` for _verbose_.
143.    Which of the following is not typically used to store shared libraries?

        1. `/lib`
        2. `/etc/lib`
        3. `/usr/lib`
        4. `/usr/local/lib`

        Answer:

        B.  The `/etc/lib` directory is not typically associated with library files and does not typically exist on a Linux system unless manually created. The other options either contain system libraries or can be used for that purpose.
144.    Which of the following commands updates the package cache for a Debian system?

        1. `apt-get cache-update`
        2. `apt-cache update`
        3. `apt-get update`
        4. `apt-get upgrade`

        Answer:

        C.  The `apt-get update` command will cause the package cache to be updated by retrieving the latest package list from the package sources. There is no `cache-update` option or `update` option to `apt-cache`. The `upgrade` option is used to update the system's packages, not the cache.
145.    You need to update the configuration files for package repositories. Within which directory are details of the current package repositories stored on a Debian system?

        1. `/etc/apt.list`
        2. `/etc/sources.list`
        3. `/etc/apt/sources.list.d/`
        4. `/etc/apt.d/sources.list`

        Answer:

        C.  The `/etc/apt/sources.list.d/` directory contains repositories for Debian packages. The other file and directory locations do not exist by default.
146.    Which of the following commands is used to change the keyboard layout settings?

        1. `keybrdctl`
        2. `keyctl`
        3. `localectl`
        4. `localemap`

        Answer:

        C.  The `localectl` command is used to view and configure settings such as the keyboard layout for a given locale. The other commands listed do not exist.
147.    Which of the following directories contains configuration files related to networking?

        1. `/etc/netdevices/`
        2. `/etc/netcfg/`
        3. `/etc/config/network/`
        4. `/etc/sysconfig/network-scripts/`

        Answer:

        D.  The directory `/etc/sysconfig/network-scripts` contains files related to network configuration. It is not preferable to edit these files directly any longer but rather to use commands such as `nmcli` and `nmtui` through the Network Manager. The other paths do not exist by default.
148.    You need to change the label that has been applied to a filesystem. The filesystem is formatted as `EXT4`. Which `EXT` tool can be used to change the label?

        1. `e2label`
        2. `e4label`
        3. `fslabel.ext4`
        4. `fslabel`

        Answer:

        A.  The `e2label` command changes the filesystem label. The other commands do not exist.
149.    Which command should be used to make changes to the choices made when a Debian package was installed?

        1. `dpkg-reconfigure`
        2. `dpkg -r`
        3. `dpkg ––reconf`
        4. `apt-get reinstall`

        Answer:

        A.  The `dpkg-reconfigure` program will cause an already-installed package to be reconfigured or changed. The `-r` option for `dpkg` removes a package, thus making option B incorrect. There is no `reconf` option for `dpkg` or `reinstall` option for `apt-get`.
150.    Which option for `yum` performs a search of the package cache?

        1. `seek`
        2. `query`
        3. `––search`
        4. `search`

        Answer:

        D.  The `search` option performs a search of various fields such as the package name and description.
151.    Assume you need to add a kernel module with a custom command, such as to specify options at load time. Within which file could you add this configuration?

        1. `/etc/modprobe-cfg`
        2. `/etc/modprobe.conf`
        3. `/etc/modprobe.cf`
        4. `/etc/modprobe.cfg`

        Answer:

        B.  The file `/etc/modprobe.conf`, which is a legacy file and may be removed in a later version of Linux, contains information on the configuration of modules on the system. The other files do not exist.
152.    Which command option for `rpm` can be used to show the version of the kernel?

        1. `rpm kernel`
        2. `rpm -q kernel`
        3. `rpm search kernel`
        4. `rpm ––list kern`

        Answer:

        B.  The `rpm -q kernel` command will show the kernel version. You can also use `uname -r` for the same purpose.
153.    Which command is used to install a kernel into the `/boot` directory, using the files from `/usr/lib/kernel`?

        1. `kernel-ins`
        2. `ins-kernel`
        3. `install-kernel`
        4. `kernel-install`

        Answer:

        D.  The `kernel-install` command uses the files found in the `/usr/lib/kernel` directory to install a kernel and related files into `/boot`. The other commands listed here are not valid.
154.    Which option in `/etc/yum.conf` is used to ensure that the kernel is not updated when the system is updated?

        1. `exclude=kernel*`
        2. `exclude-kernel`
        3. `updatekernel=fals`e
        4. `include-except=kernel`

        Answer:

        A.  The `exclude` option can be used to exclude certain packages. The argument accepts wildcards, and therefore excluding all `kernel*` updates will create the desired behavior.
155.    When using `fdisk` to partition a disk, you have two partitions created for the system but still have leftover space, also called unallocated space, on the drive. What is another name used to refer to unallocated space?

        1. Highly available
        2. Redundant
        3. Raw device
        4. Partition forward

        Answer:

        C.  A raw device is one that has not been partitioned. Raw devices are sometimes used for virtualization and also database scenarios, where the higher-layer software manages the disk. The other options shown are not relevant to this answer. Highly available would only typically refer to a redundant disk or network scenario.
156.    Which command searches for and provides information on a given package on a Debian system, including whether the package is currently installed?

        1. `dpkg -i`
        2. `dpkg -s`
        3. `apt-cache`
        4. `apt-info`

        Answer:

        B.  The `-s` option to `dpkg` searches for the given package and provides information about its current status on the system. The `apt-cache` command is not used for this purpose, and the `-i` option for `dpkg` installs a package. The `apt-info` command does not exist.
157.    Which of the following installs a previously downloaded Debian package?

        1. `dpkg -i <package name>`
        2. `apt-install <package name>`
        3. `apt-slash <package name>`
        4. `dpkg -U <package name>`

        Answer:

        A.  The `-i` option to `dpkg` will install a previously downloaded `.deb` Debian package. The other commands don't exist, and the `-U` option for `dpkg` does not exist.
158.    You need to obtain information about a package installed on an OpenSUSE system that uses the `zypper` command. Which of the following options to the `zypper` command displays information about the package?

        1. `inf`
        2. `getInfo`
        3. `info`
        4. `i`

        Answer:

        C.  The `info` option displays information about a given package on a system that uses the `zypper` tool.
159.    Which type of storage would be the most appropriate format to store a large object as a single file in a cloud environment?

        1. File
        2. ext2
        3. cifs
        4. Blob

        Answer:

        D.  Blob, or Binary Large Object, is a storage format frequently associated with cloud environments. Blob storage enables a single object to be stored as an individual object. The other formats are valid, but none of the other options is the most appropriate mechanism for this scenario. File storage refers to the hierarchy of folders and files that you would see when using a command like `ls`.
160.    You need to find available packages on a Fedora system managed by the `dnf` package system. Which option to the `dnf` command looks for a given package?

        1. `search`
        2. `info`
        3. `find`
        4. `locate`

        Answer:

        A.  The `search` option looks for packages by the name given on the command line. The path that is searched can be controlled by the configuration file at `/etc/dnf/dnf.conf`. The other options are not valid for the `dnf` command.
161.    Which of the following real filesystems can be resized using `resize2fs`?

        1. `nfs`
        2. `xfs`
        3. `ext3`
        4. `cifs`

        Answer:

        C.  The `ext2`, `ext3`, and `ext4` filesystems can be resized using `resize2fs`. Both NFS and CIFS are network filesystems and therefore are not relevant to this question.
162.    Which subcommand to the `virsh` command is used to connect to the hypervisor?

        1. `plug`
        2. `hypervisorconnect`
        3. `conhyper`
        4. `connect`

        Answer:

        D.  The `connect` subcommand connects to the hypervisor. The other options are not valid subcommands for `virsh`.
163.    You need to determine if ASCII and Unicode are supported on the system. Which option to the `iconv` command shows the available character sets on a given system?

        1. `--showchar`
        2. `--show`
        3. `--list`
        4. `--all`

        Answer:

        C.  The `--list` option shows the available character sets on the system. Character sets such as ASCII, UTF-8, and UNICODE are displayed if they are supported on the system. The other options given for this question do not exist.
164.    Which of the following best describes the `/dev/` filesystem?

        1. The `/dev/` filesystem is used for storing device information for connected devices.
        2. The `/dev/` filesystem is used for configuration files.
        3. The `/dev/` filesystem is used for development.
        4. The `/dev/` filesystem is used to list devices for compilation into the kernel.

        Answer:

        A.  The `/dev/` filesystem is used to store information about connected devices, including block and character devices. The `/dev/` filesystem also contains special character devices such as `/dev/null`, `/dev/zero`, and `/dev/urandom`. The `/etc/` filesystem is used for configuration files, and there are no proscribed directories for development or kernel device lists.
165.    Which of the following files shows the currently mounted filesystems?

        1. `/etc/fstab`
        2. `/proc/mounts`
        3. `/fs`
        4. `/root/mounts`

        Answer:

        B.  The `/proc/mounts` file shows the currently mounted filesystems. The file `/etc/fstab` is used for mounting filesystems but is not kept up-to-date with filesystem mounts as they change. The other files listed do not exist.
166.    When working with a Microsoft Windows–based filesystem, you see that it is mounted as a CIFS mount. What does CIFS stand for?

        1. Common Information File Sharing
        2. Common Internet File System
        3. Cloned Internet File Sharing
        4. Created In Five Seconds

        Answer:

        B.  CIFS is the Common Internet File System and is now considered a legacy filesystem, having been superseded by SMB3. CIFS is an implementation of SMB typically used by older versions of Microsoft Windows.
167.    When using `sed` for a substitution operation, which option must be included so that the substitution applies to the entire line rather than just the first instance?

        1. `g`
        2. `a`
        3. `r`
        4. `y`

        Answer:

        A.  The `g` option, also known as `global` or `greedy`, will apply the matched operation to the entire line rather than just the first instance of the match. The other options apply as they would for a Perl Compatible Regular Expression.
168.    Which option to the `blkid` command purges the cache to remove devices that do not exist?

        1. `-p`
        2. `-a`
        3. `-g`
        4. `-m`

        Answer:

        C.  The `-g` option clears the cache to remove devices that do not exist. The `-p` option bypasses the cache. There are no `-a` or `-m` options for `blkid`.
169.    While you can use `blkid` to obtain the UUIDs for filesystems in order to facilitate storage space monitoring and disk usage, which location on the filesystem also shows this information?

        1. `/dev/diskbyuuid`
        2. `/dev/uuid`
        3. `/dev/fs/uuid`
        4. `/dev/disk/by-uuid`

        Answer:

        D.  The `/dev/disk/by-uuid` file shows the UUID of the disks on a system. The other locations do not exist.
170.    In a scripting scenario, you need to enable legacy locations for things like networking. Which file can be used for storing network configuration?

        1. `/etc/netdev`
        2. `/etc/networking`
        3. `/etc/sysconfig/network`
        4. `/etc/sysconfig/netdev`

        Answer:

        C.  The `/etc/sysconfig/network` file is created by default but is no longer populated on systems like RHEL7. It can be used in place of Network Manager for environments that rely on this location. The other options given for this question do not exist.
171.    You are attempting to use `rmdir` to remove a directory, but there are still multiple files and other directories contained within it. Assuming that you're sure you want to remove the directory and all of its contents, what are the command and arguments to do so?

        1. `rm -f`
        2. `rm -rf`
        3. `rmdir -a`
        4. `rmdir -m`

        Answer:

        B.  The `-rf` options to `rm` will recursively remove contents of a directory, including other directories. The `-f` option alone will not work in this case because of the additional directories. The options given for `rmdir` do not exist.
172.    Which of the following commands will provide the usernames in a sorted list gathered from the `/etc/passwd` file?

        1. `cat /etc/passwd | awk -F : '{print $1}' | sort`
        2. `sort /etc/passwd | cut`
        3. `echo /etc/passwd`
        4. `cat /etc/passwd | awk '{print $1}' | sort`

        Answer:

        A.  The `cat` command will display the contents of the file `/etc/passwd` and then pipe that output to the `awk` command. The `awk` command then parses its input, splitting along the specified separator for `/etc/passwd`, which is a colon (`:`). The output is then printed and piped to the `sort` command. The `sort` command in option B will not work because the `cut` command requires an argument. Likewise, the `echo` command in option C will only `echo /etc/passwd` to `STDOUT`.
173.    What will be the result if the `touch` command is executed on a file that already exists?

        1. The access timestamp of the file will change to the current time when the `touch` command was executed.
        2. The file will be overwritten.
        3. There will be no change.
        4. The file will be appended to.

        Answer:

        A.  The timestamp of the file will change when `touch` is run on a file that already exists.
174.    Which option to both `mv` and `cp` will cause the command to prompt before overwriting files that already exist?

        1. `-f`
        2. `-Z`
        3. `-r`
        4. `-i`

        Answer:

        D.  The `-i` option will cause both `cp` and `mv` to be interactive, that is, prompt before overwriting. The `-f` option will force the command to run, while `-r` is recursive.
175.    Which file contains the current list of partitions along with their major and minor numbers and the number of blocks?

        1. `/dev/disk`
        2. `/dev/partitions`
        3. `/proc/disk`
        4. `/proc/partitions`

        Answer:

        D.  The `/proc/partitions` file contains a list of partitions on the system along with their major and minor numbers and the number of blocks. The `/dev/disk/` option is a directory and not a file and so is not correct for this question. The other options shown do not exist.
176.    Assuming a block storage device used for virtualization of `sda`, which file can be used to view the number of read I/O requests for the device?

        1. `/proc/sys/sda`
        2. `/proc/sys/sda/stat`
        3. `/sys/block/sda/stat`
        4. `/sys/disk/sda/stat`

        Answer:

        C.  The file `/sys/block/sda/stat` contains information about the `sda` device. The `/sys/block` hierarchy contains information about block devices on the system.
177.    The current hierarchy on the server contains a directory called `/usr/local`. You need to create an additional directory below that called `/usr/local/test/october`. Which command will accomplish this task?

        1. `mkdir -p /usr/local/test/october`
        2. `mkdir /usr/local/test/october`
        3. `mkdir -r /usr/local/test/october`
        4. `mkdir -f /usr/local/test/october`

        Answer:

        A.  The `-p` option will cause `mkdir` to create additional levels of directories without error. Running `mkdir` without options will not work in this case. The `-r` and `-f` options to `mkdir` do not exist.
178.    What command is used to bring a command to foreground processing after it has been backgrounded with an `&`?

        1. `bg`
        2. `fore`
        3. `4g`
        4. `fg`

        Answer:

        D.  The `fg` command will bring a command to the foreground if it has been backgrounded with either `&` or the `bg` command.
179.    You are using the Vi editor to change a file, and you need to exit. You receive a notice indicating “No write since last change.” Assuming you want to save your work, which of the following commands will save your work and exit Vi?

        1. `:wq`
        2. `:q!`
        3. `dd`
        4. `x`

        Answer:

        A.  You need to write the changes to the file, so you'll need `:w`. The addition of `q` will also quit. Note that you could use `ZZ` to write and quit as well. The `dd` command in Vi deletes a line, while `x` deletes a single character.
180.    When using a multipath device managed by `multipathd` and found in `/dev/disk/by-multipath`, what is the name given to the identifier for that device that is globally unique?

        1. UUID
        2. WWID
        3. GUID
        4. DISKID

        Answer:

        B.  The WWID, or Worldwide Identifier, is globally unique. UUID and GUID are not valid acronyms for multipath devices. UUID is typically found for plain block devices, and GUID is a term sometimes used in applications. There is no DISKID name relevant as a potential answer for this question.
181.    You have attempted to stop a process using its `service` command and also using the `kill` command. Which signal can be sent to the process using the `kill` command in order to force the process to end?

        1. `-15`
        2. `-f`
        3. `-9`
        4. `-stop`

        Answer:

        C.  The `-9` option invokes `SIGKILL`, which will force the process to end. The `15` signal is the default. The `-f` and `-stop` options do not exist.
182.    When editing with Vi, which command changes into insert mode and opens a new line below the current cursor location?

        1. `f`
        2. `a`
        3. `o`
        4. `i`

        Answer:

        C.  The `o` command opens a new line below the current cursor location. The `a` command begins an insert-mode session at the character after the cursor, not the line. The `i` command begins an insert-mode session at the current cursor location.
183.    While recovering from a kernel panic and using the console, you are having difficulty working with the console due to continual messages being displayed on the console itself. Which option to `dmesg` can be used to disable logging to the console?

        1. `-o “no logging console”`
        2. `-D`
        3. `-Q`
        4. `-F`

        Answer:

        B.  The `-D` option tells `dmesg` to stop displaying messages to the console. The `-F` option is valid but is used to read from a file, so it is not relevant for this question. There are no `-o` or `-Q` options.
184.    Which option to `rmmod` forces the module to be unloaded?

        1. `-f`
        2. `-a`
        3. `-w`
        4. `-h`

        Answer:

        A.  The `-f` option forces unload of the module. The other options are not valid for `rmmod`.
185.    Which command-line option modifies the behavior of `depmod` such that only newer modules are added when comparing `modules.dep`?

        1. `-A`
        2. `-B`
        3. `-C`
        4. `-D`

        Answer:

        A.  The `-A` option examines `modules.dep` for newer modules rather than regenerating the file automatically if there are no changes. The `-C` option changes the configuration file location. The other options are not valid for `depmod`.
186.    Which command prints device and partition information in a tree-like structure, including partition size and current mount status?

        1. `fsck`
        2. `lsblk`
        3. `blkshow`
        4. `shblk`

        Answer:

        B.  The `lsblk` command shows device information in a tree-like structure and shows the other information specified along with major and minor information and whether the partition is read-only. Of the other options given, `fsck` is the only command, and it is not used for the purpose described.
187.    You need to create a script for use with the `parted` command. When using the `parted` command to obtain a list of partitions, which additional option formats the output such that it can be more easily parsed by a script?

        1. `-p`
        2. `-S`
        3. `-m`
        4. `-v`

        Answer:

        C.  The `-m` option displays output in a machine-readable format. The `-v` option prints the version of `parted`. There is no `-p` or `-S` option.
188.    Which command is used to create an Ethernet bridge?

        1. `bridgecon`
        2. `brctl`
        3. `bridgeman`
        4. `BridgeManager`

        Answer:

        B.  The `brctl` command is used to create ethernet bridges and is also used to manage bridges once they are created. The other options shown are not valid.
189.    Which kill signal can be sent in order to restart a process?

        1. `-HUP`
        2. `-RESTART`
        3. `-9`
        4. `-SIG`

        Answer:

        A.  Sending `-HUP` as part of the `kill` command will restart a process. Of the other options, `-9` will kill the process completely. The other two options do not exist as valid means to kill a process.
190.    Which command will move all files with a `.txt` extension to the `/tmp` directory?

        1. `mv txt* tmp`
        2. `move *txt /temp`
        3. `mv *.txt /tmp`
        4. `mv *.txt tmp`

        Answer:

        C.  The `mv` command is used to move files, and `*.txt` will look for all files with a `.txt` extension. Note the fully qualified destination with a `/` preceding the name `tmp`.
191.    When using `nslookup` interactively, which of the following commands changes the destination to which queries will be sent?

        1. `dest`
        2. `server`
        3. `queryhost`
        4. `destination`

        Answer:

        B.  The `server` command changes the destination for queries sent from `nslookup` during the session in which it's used. The other options shown are not valid.
192.    Another administrator made a change to one of the local scripts stored in `/usr/local/bin` and used for administrative purposes. The change was also immediately reflected in the copy of the script in your home directory. However, when you examine the file with `ls`, it appears to be a normal file. What is the likely cause of such a scenario?

        1. The file was executed after edit.
        2. The administrator copied the file to yours.
        3. Your file is a hard link to the original.
        4. The file has been restored from backup.

        Answer:

        C.  The file is almost certainly a hard link to the original script. While `ls` won't show this information, the `stat` command will show that it is a link and also show the inode to which the file is linked.
193.    Which option to `ln` creates a symlink to another file?

        1. `-sl`
        2. `-s`
        3. `-l`
        4. `--ln`

        Answer:

        B.  The `-s` option to `ln` creates a symbolic link, or symlink.
194.    When using `ls -la` to obtain a directory listing, you see an object with permissions of `lrwxrwxrwx`. What type of object is this?

        1. It is a directory.
        2. It is a symlink.
        3. It is a temporary file.
        4. It is a local file.

        Answer:

        B.  The `l` within the listing indicates a symlink. There is no way to tell if a file or directory is temporary. A directory will display a `d` instead of an `l`.
195.    On a system using SysVinit as part of the basic boot process, in which directory are startup and shutdown scripts for services stored?

        1. `/etc/init-d`
        2. `/etc/init`
        3. `/etc/sysV`
        4. `/etc/init.d`

        Answer:

        D.  Scripts are stored in `/etc/init.d` on a system using SysVinit. You may sometimes find these linked from `/etc/rc.d/init.d` as well. The other options are not valid for this question.
196.    Which option to the `cp` command will copy directories in a recursive manner?

        1. `-v`
        2. `-R`
        3. `-Z`
        4. `-i`

        Answer:

        B.  The `-R` option will copy directories recursively. Note that if the `-i` option is not enabled, the recursive copy will overwrite files in the destination. The `-v` option adds verbosity but does not cause any recursion, while the `-Z` option does not exist.
197.    Which option to `df` displays the output in human-readable format?

        1. `-h`
        2. `-m`
        3. `-j`
        4. `-s`

        Answer:

        A.  The `-h` option displays output in human-readable format, meaning that the output will be displayed as megabytes, gigabytes, terabytes, and so on. The other options are not valid.
198.    Which command creates a TCP connection to the server `www.example.com` on port 80?

        1. `nc` `www.example.com` 80
        2. `nc` `www.example.com`
        3. `nc` `www.example.com:80`
        4. `nc:80` `www.example.com`

        Answer:

        A.  The `netcat` tool used with the `nc` command can create a network connection, and the format is `nc <host> <port>`, thus making options other than that incorrect.
199.    Which option to the `file` command specifies that `file` should examine compressed files?

        1. `-a`
        2. `-z`
        3. `-w`
        4. `-b`

        Answer:

        B.  The `-z` option causes `file` to look inside compressed files. The `-b` option specifies brief output, and the other options don't exist.
200.    Which option to Vim enables editing of binary or executable files?

        1. `-a`
        2. `-b`
        3. `-c`
        4. `-d`

        Answer:

        B.  The `-b` option enables binary and executable editing with Vim. The `-c` option is related to commands, while the `-d` option starts Vim in diff mode. There is no `-a` option.
201.    When using the `rmdir` command, which option also removes child directories?

        1. `-c`
        2. `-p`
        3. `-m`
        4. `-a`

        Answer:

        B.  The `-p` option removes the hierarchy of directories. The other options do not exist.
202.    Emptying or clearing a block device is sometimes accomplished by writing zeroes to the device. Which file is used for this purpose?

        1. `/dev/format`
        2. `/dev/go`
        3. `/dev/zero`
        4. `/tmp`

        Answer:

        C.  The `/dev/zero` special file is used as input to the `dd` command to write zeros or clear a block device. The other options either do not exist or are not used for this purpose.
203.    Which option to `zip` updates files within the archive but does not add files?

        1. `-a`
        2. `-f`
        3. `-d`
        4. `-e`

        Answer:

        B.  The `-f` option freshens the files within the archive. The `-d` option deletes from the archive. The other options do not exist.
204.    Which of the following will execute a job through `cron` at 12:15 a.m. and 12:15 p.m. every day?

        1. `0,12 15 * * *`
        2. `15 0,12 * * *`
        3. `15 * * * 0/12`
        4. `*/12 * * * 15`

        Answer:

        B.  The format for `cron` is \[`minute hour day-of-month month-of-year day-of-week`], thereby making option B the correct option for this question.
205.    Which file is used to provide a list of users that can add and delete `cron` jobs?

        1. `/etc/cron.job`
        2. `/etc/cron.allow`
        3. `/etc/cron.users`
        4. `/etc/crontab`

        Answer:

        B.  The `/etc/cron.allow` file is a list of users who have permission to create and remove their own `cron` jobs. The `/etc/crontab` file is used to store `cron` jobs. The other files do not exist.
206.    Which of the following commands schedules a series of commands to execute one hour from now?

        1. `atq +1hr`
        2. `at now + 1 hour`
        3. `atq`
        4. `at -1`

        Answer:

        B.  The `at` command is used to run a series of commands that you enter. Unlike with `cron`, you can schedule commands from the command line to be executed in the same order entered rather than having to create a specific script for the commands. The syntax shown in option B sets the time to be one hour from now.
207.    Which of the following best describes the `/proc` filesystem?

        1. `/proc` contains information about files to be processed.
        2. `/proc` contains configuration files for processes.
        3. `/proc` contains information on currently running processes, including the kernel.
        4. `/proc` contains variable data such as mail and web files.

        Answer:

        C.  The `/proc` filesystem contains information about currently running processes and additional information about the kernel and current boot of the system.
208.    Which option to `fdisk` provides a list of partitions on a given device?

        1. `-s`
        2. `-l`
        3. `-e`
        4. `-d`

        Answer:

        B.  The `-l` option lists partitions available on a given device. The `-s` option prints the size in 512-byte block sectors. The other options do not exist.
209.    Within which directory would you find a list of files corresponding to the users who have current `cron` jobs on the system?

        1. `/var/spool/cron/crontabs`
        2. `/var/spool/jobs`
        3. `/etc/cron`
        4. `/etc/cron.users`

        Answer:

        A.  The `/var/spool/cron/crontabs` directory contains a file for each user that currently has one or more `cron` jobs or entries. Note that the other files listed here are not valid for this purpose.
210.    Which command deletes an `at` job with an ID of 3?

        1. `atq`
        2. `at -l`
        3. `atrm 3`
        4. `rmat 3`

        Answer:

        C.  The `atrm` command removes jobs given their ID. The ID can be obtained with the `atq` command. The `atq` and `at -l` commands shown will list jobs but not delete them. The `rmat` command is not valid.
211.    Which of the following is used as a system-wide `cron` file?

        1. `/etc/cron.d`
        2. `/etc/cron.sys`
        3. `/etc/crontab`
        4. `/etc/cron.tab`

        Answer:

        C.  The `/etc/crontab` file is a plain-text file that is treated as a system-wide `cron` file. As such, the file is generally not associated with any single user, and it's not necessary to run a special command after editing this file.
212.    Within which directory will you find scripts that are scheduled to run through `cron` every 24 hours?

        1. `/etc/cron.daily`
        2. `/etc/cron.weekly`
        3. `/etc/cron.hourly24`
        4. `/etc/crontab`

        Answer:

        A.  The `/etc/cron.daily` directory contains files such as scripts that are executed daily. There are corresponding `cron.hourly`, `cron.weekly`, and `cron.monthly` directories that run on their respective schedules as indicated by the name of each directory.
213.    The system that you're working with recently had a hard drive failure, resulting in degraded storage. A new hard drive has been installed and Linux has been restored from backup to the drive. However, the system will not boot and instead shows a `grub >` prompt. Within the `grub >` prompt, which command will show the current partitions as seen by GRUB?

        1. `ls`
        2. `showPart`
        3. `partitionlist`
        4. `ps`

        Answer:

        A.  The `ls` command from within the `grub >` prompt will show the available partitions in a format such as `(hd0,1)`.
214.    A legacy PATA disk is used to boot the system. You recently added an internal DVD drive to the computer, and now the system will no longer boot. What is the most likely cause?

        1. The BIOS has identified the DVD drive as the first disk, and therefore the system can no longer find the Linux partition(s).
        2. The hard drive became corrupt when the DVD drive was installed.
        3. The hot swap option has not been enabled in the BIOS.
        4. The DVD drive is not detected by the computer and needs to be enabled first in the BIOS and then in Linux prior to installation.

        Answer:

        A.  With cable select, ATA drives will be detected in the order in which they are plugged in on the cable from the motherboard. It's likely that the drives need to be swapped physically on the cable.
215.    Which of the following will run a command called `/usr/local/bin/changehome.sh` as the `www-data` user when placed in `/etc/crontab`?

        1. `1 1 * * * www-data /usr/local/bin/changehome.sh`
        2. `www-data changehome.sh`
        3. `*/1 www-data changehome.sh`
        4. `* * */www-data /usr/local/bin/changehome.sh`

        Answer:

        A.  The format when adding a username places the username between the schedule and the command to run, thereby making option A correct. The other options shown for this question are invalid. In the case of option B, there is no schedule. In the case of options C and D, the schedule is incorrectly formatted.
216.    Which command and option are used to update a Debian system to the latest software?

        1. `apt-update`
        2. `apt-get upgrade`
        3. `dpkg -U`
        4. `apt-cache clean`

        Answer:

        B.  The `upgrade` option for `apt-get` will upgrade the system to the latest version of software for packages already installed. The `apt-update` command does not exist, nor does the `-U` option to `dpkg`. The `apt-cache` command is used to work with the package cache.
217.    You need to write a script that gathers all the process IDs for all instances of Apache running on the system. Which of the following commands will accomplish this task?

        1. `ps auwx | grep apache`
        2. `pgrep apache`
        3. `processlist apache`
        4. `ls -p apache`

        Answer:

        B.  While the `ps auwx` command combined with `grep` will provide information on the running Apache instances, it will provide much more information than is required or useful for this problem. The `pgrep` command provides only the process IDs and therefore meets the criteria presented in the question.
218.    Which command can be run to determine the default priority for processes spawned by the current user?

        1. `prio`
        2. `nice`
        3. `renice`
        4. `defpriority`

        Answer:

        B.  The `nice` command, when run without arguments, will output the priority for the currently logged-in user, which is normally 0. The `renice` command can be used to change the priority of running processes. The other two commands shown as options for this question do not exist.
219.    Which of the following commands shows the usage of inodes across all filesystems?

        1. `df -i`
        2. `ls -i`
        3. `du -i`
        4. `dm -i`

        Answer:

        A.  The `-i` option to `df` produces information on inodes across all filesystems. The `ls -i` option will produce inode listings but only for the current directory. The `-i` option is invalid for `du`, and `dm` does not exist as a command.
220.    Which command will list the `cron` entries for a given user as denoted by `<username>`?

        1. `crontab -l -u <username>`
        2. `crontab -u <username>`
        3. `cron -u <username>`
        4. `cronent -u <username>`

        Answer:

        A.  The `crontab` command can be used for this purpose, and the `-l` option is used to list the `crontab` entries. The `-u` option is needed to specify a user other than the current user.
221.    You are having difficulty with an interface on the server, and it is currently down. Assuming that there is not a hardware failure on the device itself, which command and option can you use to display information about the interface?

        1. `ifconfig -a`
        2. `ifup`
        3. `netstat -n`
        4. `ifconfig`

        Answer:

        A.  The `ifconfig` command will be used for this purpose and requires the addition of the `-a` option because the adapter is currently down. The `ifup` command can be used to bring up an interface but does not display information by default. The `netstat` command displays information about the network but not with the `-n` option.
222.    Which option to the `traceroute` command will use TCP SYN packets for the path trace?

        1. `-T`
        2. `-t`
        3. `-s`
        4. `-i`

        Answer:

        A.  The `-T` option causes `traceroute` to use TCP packets. This option, which requires root privileges, can be helpful for situations where a firewall may be blocking `traceroute` traffic. The `-i` option chooses the interface, while `-s` chooses the source address. A lowercase `-t` option sets the Type of Service (ToS) flag.
223.    When troubleshooting an issue where SSH connections are timing out, you think the firewall is blocking SSH connections. Which of the following ports is used for Secure Shell communication?

        1. TCP/23
        2. TCP/25
        3. TCP/22
        4. TCP/2200

        Answer:

        C.  Secure Shell, or SSH, operates on TCP port 22 by default. TCP/23 is used for Telnet, TCP/25 is SMTP, and TCP/2200 is not associated with a well-known service.
224.    Which options for `netcat` will create a server listening on port 8080?

        1. `netcat -p 8080`
        2. `nc -l -p 8080`
        3. `nc -p 8080`
        4. `nc -s 8080`

        Answer:

        B.  The `nc` command is used to start `netcat`, and the `-l` option causes it to listen. The `-p` option is used to specify the port on which `netcat` will listen. The `-s` option specifies the local source address and is not used for this scenario.
225.    Which of the following commands displays the Start of Authority information for the domain [`example.com`](http://example.com/)?

        1. `dig` [`example.com`](http://example.com/) `soa`
        2. `dig` [`example.com`](http://example.com/) `authority`
        3. `dig` [`example.com`](http://example.com/) `-auth`
        4. `dig -t auth` [`example.com`](http://example.com/)

        Answer:

        A.  The `soa` type is used to query for Start of Authority records for a domain. Note that in many cases, `dig` will attempt to look up the domain within a given command and may not appear to have had an error. For example, when running option D (`dig -t auth` [`example.com`](http://example.com/)), you will receive information about [`example.com`](http://example.com/), and there will be a line in the output that `dig` has ignored the invalid type `auth`.
226.    When configuring a local NTP server role, to what server address can you set the server's NTP client?

        1. `127.0.0.1`
        2. `192.168.1.100`
        3. `ntp.example.com`
        4. [`pool.ntp.org`](http://pool.ntp.org/)

        Answer:

        A.  Setting your address to `127.0.0.1` will use the localhost interface. Other local NTP clients would contact this server by its normal IP address.
227.    A developer has created an application and wants to take advantage of `syslog` for logging to a custom log file. Which facility should be used for an application such as this?

        1. `syslog`
        2. `kern`
        3. `local#`
        4. `user`

        Answer:

        C.  The application could theoretically use any of the logging facilities, depending on the type of application being developed. However, the requirement to log to a custom log file means the logs will have a different name and possibly a different location than the standard logs. Therefore, logging to any of the standard or system-level facilities is not appropriate for this scenario, so one of the local (`local0` through `local7`) facilities is appropriate.
228.    You are troubleshooting a DNS problem using the `dig` command and receive a “status: NXDOMAIN” message. Which of the following best describes what NXDOMAIN means?

        1. NXDOMAIN means you have received a non-authoritative answer for the query.
        2. NXDOMAIN means the domain or host is not found.
        3. NXDOMAIN indicates a successful query.
        4. NXDOMAIN signifies that a new domain record has been added.

        Answer:

        B.  NXDOMAIN is the status for a nonexistent domain or host: basically, the host for which the query was sent does not exist. A normal status when there has not been an error is “NOERROR.”
229.    Which of the following commands can be used to restart the CUPS service after a configuration change on a server running `systemd`?

        1. `systemctl restart cups.service`
        2. `systemctl restart cups`
        3. `systemctl reboot cups.target`
        4. `systemctl restart cups.target`

        Answer:

        A.  The `systemctl` command is used for controlling services. In this case, `restart` should be sent to the CUPS service as denoted by the name `cups.service`.
230.    You need to temporarily prevent users from logging in to the system using SSH or other means. Which of the following describes one method for accomplishing this task?

        1. Run `touch /etc/nologin`.
        2. Disable `sshd`.
        3. Remove `/etc/login`.
        4. Add a shadow file.

        Answer:

        A.  If `/etc/nologin` exists, users will be prevented from logging in to the system. The root user can still log in, assuming that root logins are enabled within the SSH configuration.
231.    When expiring a user account with `usermod -e`, which of the following represents the correct date format?

        1. `YYYY-MM-DD`
        2. `MM/DD/YYYY`
        3. `DD/MM/YY`
        4. `MM/DD/YY HH:MM:SS`

        Answer:

        A.  The correct format is `YYYY-MM-DD` for the `usermod` command.
232.    Which of the following commands can be used to stop a given service, such as `httpd.service`, from starting on boot with a `systemd`-based system?

        1. `systemctl disable httpd.service`
        2. `systemctl stop httpd.service`
        3. `systemd disable httpd.service`
        4. `systemd enable httpd.service boot=no`

        Answer:

        A.  The `systemctl` command will be used for this purpose, and the subcommand is `disable`. There is a `stop` subcommand, but it will only stop the given service rather than prevent it from starting on boot. The other options are invalid for various reasons, including that they use `systemd` as the command name rather than `systemctl`.
233.    Which of the following commands searches the entire filesystem for files with the `setuid` bit set?

        1. `find ./ -perm suid`
        2. `find / -perm 4000`
        3. `find / -type suid`
        4. `find / -type f -perm setuid`

        Answer:

        B.  The `find` command will be used for this purpose, and the permission can be described as `4000` to indicate the presence of the `setuid` bit. The `-type` option can be used for changing the type of object to be returned but is not relevant for the scenario described.
234.    You are upgrading the kernel that has been previously compiled on the same server. Which of the following commands incorporates the contents of the existing kernel configuration into the new kernel?

        1. `config --merge`
        2. `make oldconfig`
        3. `merge config`
        4. `int configs`

        Answer:

        B.  The `make oldconfig` command will integrate the existing configuration file into the new configuration for the kernel. Care still needs to be taken for items that have moved or changed within the new kernel, to ensure that the configuration is correct.
235.    Which of the following commands should you execute after making changes to `systemd` service configurations in order for those changes to take effect?

        1. `systemd reload`
        2. `reboot`
        3. `systemctl daemon-reload`
        4. `systemctl reboot`

        Answer:

        C.  The `systemctl` command will be used for this purpose, with the `daemon-reload` subcommand. The `reboot` option would work to reload the `systemd` configuration but is not correct because it requires the entire server to reboot, which is not what was asked for in this question.
236.    As a system administrator, you need to change options for `automount`. Which of the following files is the default configuration file for the `autofs` automounter?

        1. `/etc/autofs`
        2. `/etc/auto.master`
        3. `/etc/autofs.conf`
        4. `/etc/automounter.conf`

        Answer:

        B.  The file `/etc/auto.master` contains the configuration for `autofs`. The other files listed as options are not valid for this scenario.
237.    Which of the following directory hierarchies contains information such as the WWN for Fibre Channel?

        1. `/sys/class/wwn`
        2. `/sys/class/fc_host`
        3. `/sys/class/fclist`
        4. `/sys/class/fc/wwn`

        Answer:

        B.  The directory `/sys/class/fc_host` contains other directories based on the Fibre Channel connections available. Within those host directories will be found the WWN (World Wide Name) in a file called `port_name`. The `fcstat` command can be used to obtain statistics related to a given device. The other directory hierarchies are not valid.
238.    Which option to the `rsync` command provides archive mode?

        1. `-r`
        2. `-o`
        3. `-a`
        4. `-f`

        Answer:

        C.  The `-a` option provides archive mode, which is a substitute for several other options. The `-r` option is recursive, the `-o` option indicates that ownership should be preserved, and the `-f` option enables a filter.
239.    When compiling software such as with the `gcc` compiler, which of the following is the recommended name for a file containing commands and relationships used with the `make` command?

        1. `Makefile`
        2. `makefile`
        3. `make.file`
        4. `Makefile.txt`

        Answer:

        A.  According to the `man(1)` page for the `make` command, the name `Makefile`, with an uppercase `M`, is the recommended name for the file. The name `makefile` is valid as a default but is not the recommended option. The other options are not valid as default names.
240.    You have downloaded a source file with the extension `.gz`. Which of the following commands will uncompress the file?

        1. `unzip`
        2. `gunzip`
        3. `dezip`
        4. `uncomp`

        Answer:

        B.  The `gunzip` command is used to uncompress files that have been compressed using gzip compression.
241.    Which target for `make`, typically included in the `makefile` for most projects, will place compiled files into their final destination and perform other operations such as making the appropriate files executable?

        1. `list`
        2. `distclean`
        3. `run`
        4. `install`

        Answer:

        D.  The `install` target installs the final compiled files in their appropriate location and makes them executable, if applicable. Of the other options, `distclean` is sometimes included as a target to return source files to their pristine state. The other targets listed are not valid.
242.    When creating a local package repository, which option within the `.repo` file in `/etc/yum.repos.d/` is used to set the URL for the repository?

        1. `url`
        2. `repourl`
        3. `httpurl`
        4. `baseurl`

        Answer:

        D.  The `baseurl` option is used to set the URL and must be fully qualified, meaning it must include the protocol, such as `http://` or `file://`.
243.    When running the `lsblk` command, there is no separate partition listed for `/boot`. From which partition is the system likely booted?

        1. There is a `/boot` partition under the `/` partition.
        2. The `/boot` partition is hidden.
        3. The system has not yet built the `/boot` partition.
        4. The `/boot` partition does not show up with `lsblk`.

        Answer:

        A.  The `/boot` partition almost certainly exists but has not been partitioned into its own space. The `/boot` partition would not be hidden from `lsblk` if it was indeed a separate partition.
244.    Which of the following commands displays the currently open ports and the process that is using the port?

        1. `netstat -a`
        2. `lsof -i`
        3. `ps auwx`
        4. `netlist`

        Answer:

        The `lsof` command can be used for this purpose; with the `-i` option, it will display the network ports along with their process. The `netstat` command will display network ports but not the process with the `-a` option. The `ps` command is used for processes but not network ports. Finally, there is no `netlist` command.
245.    Which option to the `wget` command logs output?

        1. `-r`
        2. `-o`
        3. `-b`
        4. `-k`

        Answer:

        B.  The `-o` option logs output to the file specified. The `-k` option converts links, and the `-r` option indicates recursive. There is no `-b` option.
246.    When executed on a `systemd`-enabled server, the `service status` command is equivalent to which command?

        1. `systemd status`
        2. `journald status`
        3. `service-systemd status`
        4. `systemctl status`

        Answer:

        D.  The `service status` command is equivalent to `systemctl status` on `systemd`-enabled computers. The other commands do not exist with the specified option.
247.    Which signal to the `kill` command can be used to signal that BIND should reload, including its configuration?

        1. `-15`
        2. `-1`
        3. `-9`
        4. `-2`

        Answer:

        B.  The `-1`, or `-HUP`, signal reloads the given process. The `-15` signal, also known as `SIGTERM`, is the default terminate signal, while `-2` is an interrupt signal. The `-9` signal is `kill` and is considered bad practice except in emergencies when the process doesn't respond to normal signals.
248.    You are troubleshooting a daemon process and have started the daemon manually from the command line so that it does not fork into the background. Which key combination can be used to terminate the daemon?

        1. Ctrl+A
        2. Ctrl+B
        3. Ctrl+C
        4. Ctrl+D

        Answer:

        C.  The Ctrl+C key combination terminates, or kills, a process in a scenario such as the one described here. The Ctrl+D option is a valid key combination but is used to delete the character underneath the cursor.
249.    Which service command is used to shut down a service?

        1. `shutdown`
        2. `stop`
        3. `norun`
        4. `runstop`

        Answer:

        B.  The `stop` command, when used with the `service` command, causes a given service to shut down. The service can be started again with the `service start` command. The other options shown are not valid commands to use with the `service` command.
250.    Which subcommand with `hostnamectl` can be used to set the type of machine on which it is running?

        1. `set-machine`
        2. `machine-type`
        3. `set-type`
        4. `chassis`

        Answer:

        D.  The `chassis` subcommand configures the type of machine on which the `hostnamectl` command is running. This can be useful for certain types of applications. Of the other options, the `hostname` command can be used to set the hostname. The other commands shown are not valid.
251.    Which option to the `curl` command sets the local filename to which the output will be saved?

        1. `-f`
        2. `-o`
        3. `-O`
        4. `-l`

        Answer:

        B.  The `-o` option sets the local filename. The `-O` option preserves the remote filename. The `-f` option causes `curl` to fail silently, and the `-l` option is used with FTP to cause a name-only listing.
252.    Which of the following commands searches a server for files with the `setgid` bit enabled?

        1. `find / -perm 4000`
        2. `find ./ -perm setgid`
        3. `grep setgid *`
        4. `find / -perm 2000`

        Answer:

        D.  The `find` command will be used for this purpose, and the `-perm` option is needed, specifically as the `2000` permission to indicate `setgid`. Note the use of `/` to indicate that the entire server will be searched. The `grep` command shown cannot be used for this purpose because it looks for the presence of the string `setgid` within files located in the current directory only.
253.    You need to redirect output for a long-running process but do not need to see or capture the output. To which location can you redirect output so that it does not consume disk space?

        1. A regular file
        2. `/dev/null`
        3. `/dev/random`
        4. A network interface

        Answer:

        B.  The `/dev/null` location will accept input and not consume additional disk space when output is redirected to it. The `/dev/random` device exists but is not valid for this scenario. Likewise, redirecting to a network interface or regular file does not meet the criteria for this scenario.
254.    Which target for the `service` command will cause a daemon to reread its configuration files without restarting the daemon itself?

        1. `read`
        2. `load`
        3. `start`
        4. `reload`

        Answer:

        D.  The `reload` target or command, used as part of a `service` command, causes the daemon to reload or reread its configuration files.
255.    You have executed a daemon process manually from the command line and now need to suspend the process. Which key combination can be used for this purpose?

        1. Ctrl+S
        2. Ctrl+C
        3. Ctrl+Z
        4. Ctrl+B

        Answer:

        C.  The Ctrl+Z key combination will suspend a process. The other options are not valid for this purpose. The Ctrl+C key combination kills the process.
256.    You have been asked to recommend a simple command-line-based text editor for a beginning user. Which of the following should you recommend?

        1. Vi
        2. Nano
        3. `nc`
        4. ShellRedirect

        Answer:

        B.  The Nano editor is appropriate for this scenario. While Vi is indeed a text editor, beginners typically struggle with it. The `nc` command is not used for text editing, and there is no ShellRedirect text editor.
257.    You need to ensure that a service does not start on a `systemd` system. Which `systemctl` command should be used for this purpose?

        1. `disable`
        2. `delete`
        3. `mask`
        4. `norun`

        Answer:

        C.  The `mask` command links the unit file to `/dev/null`, thereby ensuring that the service cannot run. The `disable` command deletes the symlink between `/etc/systemd` and `/lib/systemd`, but the service could still run. The other options shown are not valid.
258.    Which command can be used to print using a specially formatted string?

        1. `printf`
        2. `echo`
        3. `print`
        4. `here`

        Answer:

        A.  The `printf` command can be used to add special formatting to strings for printing. The `echo` command can be used somewhat for this purpose but is not as powerful at special-formatting capabilities as the `printf` command is. The other commands are not valid for this purpose.
259.    You need to copy a file to a remote system, but that remote system does not have FTP or any other file-sharing services running. You have the ability to SSH into the server. Which of the following commands can be used for this purpose?

        1. `scp`
        2. `ncftp`
        3. `go`
        4. `xfer`

        Answer:

        A.  The `scp` command copies or transfers a file over SSH. The `ncftp` command cannot be used for this purpose. The other commands are not valid.
260.    Which of the following describes a method for changing the sort order when using the `top` command such that the highest memory utilizers will be shown at the top of the list?

        1. Within `top`, type **`o`** and then select `mem`.
        2. Within `top`, press Shift+F, scroll to %MEM, press `s` to select, and then press Q to quit.
        3. Within `top`, press S and then select %MEM.
        4. Within `top`, press Shift+S, select %MEM, then press Q to quit.

        Answer:

        B.  Pressing Shift+F within `top` enables you to choose which columns display as well as the sort order for the columns. In the scenario described, you can view the processes using the highest amount of memory.
261.    Which option to the `fsck` command causes it to run the check even if the filesystem is apparently marked as clean?

        1. `-f`
        2. `-m`
        3. `-a`
        4. `-c`

        Answer:

        A.  The `-f` option forces `fsck` to run on an otherwise clean filesystem. This can be helpful for times when you suspect there is an error on the filesystem and need to verify as part of the troubleshooting process. This can also be helpful to prepare the filesystem for conversion, such as might be the case with a tool like `btrfs-convert`.
262.    One of your customers needs to transfer a large file and is asking for FTP to be enabled on the server. Thinking of security, what options can you offer that are more secure?

        1. USB
        2. Email (SMTP)
        3. SSL
        4. SFTP

        Answer:

        D.  SFTP would be the preferred option because it provides additional security over legacy FTP. In general terms, FTP usually should be disabled because credentials and other traffic are not encrypted. Among the other options, email (SMTP) offers no encryption, and SSL by itself does not transfer files. Because the scenario did not include details of whether the transfer was over a long distance, it is difficult to tell whether USB would be appropriate. However, the use of a USB device is frequently discouraged on servers because it can be another attack vector.
263.    You need to extract files from a backup created with an older version of HPUX. The `tar` command does not seem to work for these files. Which of the following may be able to extract from this backup?

        1. `gzip`
        2. `bzip2`
        3. `cpio`
        4. `hpb`

        Answer:

        C.  The `cpio` utility can work with various archive formats, one of which is HPUX-created archives. The `gzip` or `bzip2` command likely would not be able to open or extract from the file; those are typically used for compression and not archival purposes.
264.    You believe that the system has been broken into and files may have been changed. After taking the system offline and unmounting one of the affected partitions, what could you do next?

        1. Use `dd` to make an image of the partition to preserve it.
        2. Create a backup using `tar`.
        3. Examine the partition with `fdisk`.
        4. Use `mkfs` to reformat the partition.

        Answer:

        A.  Making a bit-level image of the partition with `dd` is a good idea in order to preserve any evidence of the break-in. Creating a backup using `tar` is a less preferred option. Examining the partition with `fdisk` would not reveal any relevant information, and reformatting the partition usually should not be done until the extent of the attack is understood.
265.    Which option to the `zip` command causes the command to traverse directories?

        1. `-g`
        2. `-m`
        3. `-r`
        4. `-a`

        Answer:

        C.  The `-r` option tells the `zip` command to traverse directories when creating the archive. The other options are not valid for this purpose.
266.    You are working on a Debian system and need to set ownership on a file such that the user used to execute Apache can write to the file. What command can you use to determine which user Apache is running as?

        1. `ps auwx | grep apache`
        2. `ls -a`
        3. `free | grep httpd`
        4. `monapache`

        Answer:

        A.  The `ps` command, when given with arguments such as `auwx`, will show all processes and the owner of those processes. Combining with the `grep` command reveals the processes with the word _apache_ in them. On other systems, this might be called `httpd` instead of `apache`, but the question specified a Debian system.
267.    When scripting for build automation, you need to run a configure script prior to running the `make` command. Which of the following will execute the configure script, assuming that it's in the same directory as the script invoking it?

        1. `configure`
        2. `./configure`
        3. `../configure`
        4. `/configure`

        Answer:

        B.  The `./configure` pattern is typically used to invoke a configure script. Option A might work, but the `build` directory is typically not in the path.
268.    Which command can be used to change the size of a logical volume when using Logical Volume Manager?

        1. `vgs`
        2. `lvresize`
        3. `vgcreate`
        4. `lvs`

        Answer:

        B.  The `lvresize` command changes the size of a logical volume. The other commands shown are valid Logical Volume Manager commands but do not solve the problem presented.
269.    Which file contains information about RAID arrays on a Linux system?

        1. `/proc/mdstat`
        2. `/raidstat`
        3. `/var/raidinfo`
        4. `/etc/raid.txt`

        Answer:

        A.  The file `/proc/mdstat` displays information regarding the RAID arrays found a system.
270.    When working with `mdadm`, which command-line argument is used to specify things like striping and parity?

        1. `--layout`
        2. `-R`
        3. `--level`
        4. `-x`

        Answer:

        A.  Parity and striping are configured using `--layout` or `-p`. The `-x` option specifies spare devices while `-R` starts the array. The `--level` option can be used to set the type of RAID, such as mirroring (RAID1) or striping (RAID5).
271.    Which command displays Desktop Management Interface information?

        1. `dmidump`
        2. `dlad`
        3. `dmid`
        4. `dmidecode`

        Answer:

        D.  The `dmidecode` command displays information related to the DMI, or Desktop Management Interface.
272.    SSHFS is an example of which type of filesystem use?

        1. Attachment
        2. Disk
        3. RAID
        4. FUSE

        Answer:

        D.  SSHFS, or Secure Shell Filesystem, is an implementation of FUSE (Filesystem in Userspace) because it allows non-privileged users to mount a remote filesystem without needing elevated privileges.
273.    Which of the following best describes `.rpmnew` and `.rpmsave` files?

        1. The `.rpmnew` file contains RPM files and their hashes while `.rpmsave` contains a list of saved hashes.
        2. The `.rpmnew` file contains new RPM files available for download while `.rpmsave` contains a list of files that have been saved locally.
        3. The `.rpmnew` file contains a list of RPM files that have changed since the last save while `.rpmsave` is a backup of the last `.rpmnew` file.
        4. The `.rpmnew` file contains a new configuration file for a package when local changes exist to the configuration file while `.rpmsave` contains the local configuration file when a new file is included in the package.

        Answer:

        D.  The `.rpmnew` and `.rpmsave` files are used to store configurations for packages that are installed, whether a new configuration file or an existing configuration file.
274.    You are using the `top` command to monitor processes and you notice that the `nc` command is consuming a lot of CPU cycles. Which command can be used to change the priority of the command?

        1. `renice`
        2. `nice`
        3. `ps`
        4. `top`

        Answer:

        A.  The `renice` command can be used to set the priority of a running process. The `nice` command can be used to set the priority, but because the `nc` command was already running, `renice` must be used. The `nc` command can be used to transfer files, so killing the process isn't a great option. The `ps` and `top` commands do not change priorities.
275.    Which command is used to create a packaged application to be distributed with Flatpak?

        1. `flatpak-builder`
        2. `flatpak-create`
        3. `flatpak-pack`
        4. `flatpak-compile`

        Answer:

        A.  The `flatpak-builder` command is used to create the application for Flatpak. The other commands do not exist.
276.    Which background process runs to maintain the list of snap packages available on an Ubuntu system?

        1. `snapper`
        2. `snapperd`
        3. `snapdaemon`
        4. `snapd`

        Answer:

        D.  The `snapd` process runs in the background and maintains the list of snap packages available.
277.    Which tool is used to create a sandboxed AppImage package?

        1. `appimagetool`
        2. `apptool`
        3. `ocon`
        4. `app-ocon`

        Answer:

        A.  The `appimagetool` command is used to create an AppImage package. The other commands are not valid.
278.    Which network-related tool combines elements of both ping and traceroute?

        1. `tcpdump`
        2. `wireshark`
        3. `mtr`
        4. `nmcli`

        Answer:

        C.  The `mtr` command combines elements of both ping and traceroute. Among the other commands, `nmcli` is the NetworkManagement manage tool for network. Both tcpdump and wireshark/tshark are used for monitoring the network.
279.    Which option to `resolvectl` specifies the protocol?

        1. `-f`
        2. `-x`
        3. `-p`
        4. `-m`

        Answer:

        C.  The `-p` option specifies the protocol with the `resolvectl` package. The other options are not valid.
280.    Which command shows the background processes related to the current shell?

        1. `jobs`
        2. `htop`
        3. `pidof`
        4. `-m`

        Answer:

        A.  The `jobs` command shows background processes related to the current shell. The `htop` command shows running processes but beyond just the current shell. The `pidof` command displays the process id of a specific process. The other options are not valid.
281.    Which of the following commands displays Media Access Control (MAC) to IP address association?

        1. `arp`
        2. `-x`
        3. `-p`
        4. `-m`

        Answer:

        A.  The `arp` command, part of the `net-tools` package, displays the known MAC addresses and IP addresses on a given machine.
282.    As root, you run the command `cd ~` followed by `pwd` to print the working directory. What is the expected output?

        1. `/home`
        2. `/root`
        3. `/sbin`
        4. `/bin`

        Answer:

        B.  The `cd ~` command changes the current directory to the home directory, which is `/root` when you are the root user. The `/home` directory is used to as the default home directory location for normal users. The `/bin` and `/sbin` directories are used for binary programs.
283.    Which command can be used to determine a file type?

        1. `file`
        2. `xz`
        3. `lsof`
        4. `prep`

        Answer:

        A.  The `file` command examines and reports the type of file based on its contents. The `xz` command is used for file compression. The `lsof` command lists open files but not types. The `pgrep` command is related to processes.
284.    When running the `ps` command you notice that a process has a `Z` in the state field. What does `Z` represent?

        1. Sleeping
        2. Running
        3. Stopped
        4. Zombie

        Answer:

        D.  A process in Zombie state will have a state of `Z` in the output for ps. The other states shown are valid process states but not with `Z` in the output for `ps`.
285.    You need to kill a process using its name rather than its process id. Which command can be used for this purpose?

        1. `pkill`
        2. `pend`
        3. `pterminate`
        4. `kp`

        Answer:

        A.  The `pkill` command is used to terminate a process by name. The other commands shown are not valid.
286.    You need to change directory one level up from the current directory. Which command accomplishes this task?

        1. `cd .`
        2. `cd ~`
        3. `mv ~`
        4. `cd ..`

        Answer:

        D.  Using `cd` with `..` changes up one level. Using `cd` with `.` does not change directory. Using `cd` with `~` changes to the home directory, and the `mv ~` command is incomplete and does not work for the scenario provided.
