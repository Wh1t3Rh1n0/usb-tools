usb-tools
=========
Tools for Quickly Formatting and Partitioning USB Flash Drives

The rest of this file was automatically generated with the following command:

        (for f in * ; do ./$f --help ; done) >> README.md


format-usb
----------
Quickly create an msdos partition table and a single, formatted partition
on a given USB flash drive so that it is compatible with Microsoft Windows.

Usage: 

        format-usb [device] [optional partition label] [optional fs type]

You must provide a label if specifying the filesystem type.

Accepted filesystem flags:

        --ntfs
        --exfat
        --none


mkkaliusb
---------
Create a Kali or Ubuntu Linux USB flash drive with the following 
characteristics:

* A single FAT32 filesystem - The entire flash drive is still readable and
  writable from Windows and other operating systems.

* Bootable on legacy PCs via BIOS and modern PCs and Macs via EFI.

* All boot files have the hidden, system, and read-only flags set so they
  are not visible by default on Windows operating systems.

Usage:

        mkkaliusb [ISO] [device] <optional FS label>


mkwinusb
--------
Create a bootable USB Windows 7, 8, or 10 install media from an ISO.

Usage:

        mkwinusb [ISO] [device] <optional FS label>

