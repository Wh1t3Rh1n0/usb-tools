usb-tools
=========
Tools for Quickly Formatting and Partitioning USB Flash Drives

The rest of this file was automatically generated with the following command:
        (for f in * ; do ./$f --help | sed -E 's/^## ?//g' ; done) >> README.md


format-usb
----------
Quickly create an msdos partition table and a single, FAT32 filesystem
on a given USB flash drive for use with Windows.

Usage: format-usb [device] [optional partition label] [optional fs type]

You must provide a label if specifying the filesystem type.

Accepted filesystem flags:
   --ntfs
   --exfat
   --none


mkwinusb
--------
Create a bootable USB Windows 7, 8, or 10 install media from an ISO

Usage: mkwinusb [ISO] [device] <optional FS label>

