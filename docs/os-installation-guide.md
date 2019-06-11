# OS Installation Guide
RavanOS Common Linux Edition Installation Guide.

This guide will provide you all necessary information to install RavanOS common linux edition in your physical and virtual hardware.

## General OS Provisions

General-purpose operating system "RavanOS Linux Common Edition”  is a universal Linux distribution intended for
ensuring the functionality of modern computers in solving a wide range of custom tasks.

First you need  to download installation DVD-ROM from RavanOS Linux Common Edition at https://mirror.ravanos.org/common/iso.
This installation media contain an operating system boot module together with all necessary files to complete the installation process into a harddisk of the target computer. The OS can also be installed from a USB drive or over a network installation server.

## System Requirements

The OS supports parallel use of multiple processors, so-called Symmetric Multi-Processing (SMP). When the OS boots, the kernel will automatically determine the number of processors (or kernels).

To enable the console terminal to work during installation, you need a VGA compatible video interface. C-VGA is compatible with almost any modern video card.

GUI support in the installed OS is fully determined by X.Org X11 system. Most AGP, PCI and PCIe cards work under X.Org.
The installer contains all the network card drivers supported by the kernel which rum Linux kernel version 4.15.xx. This applies to almost all PCI and PCMCIA cards. To perform the installation of the OS  at least with the base configuration, the computer must have at least 1 GB of RAM  and at least 4 GB of free hard disk space drive.

## Preparation for Installation

Before you start installing the OS on the target computer, it is recommended to perform the following necessary actions:

1. Make a backup copy of existing data and documents stored on the hard disk on which you plan to install.

2. Allocate space on the hard disk under the installed OS.

3. Prepare a DVD with the OS distribution.

4. Copy the necessary files to the USB disk from the OS installation DVD if you plan to install using USB disk.

5. Carry out ,if necessary, the BIOS setup of the target computer to ensure Cookies can be downloaded from the selected media.

## Sequence of Basic Steps in Installing the Os

Actions that must be performed to install the OS:

1.  Download the OS installer from the media.

2. Select the installation program and hardware settings.

3. Activate ,if any, the connection to the Ethernet network.

4. Create an administrator account and password.

5. Adjust the time.

6. Create and mount disk partitions on which the OS will be installed.

7. Select and install the necessary software.

8. Select and install additional OS settings.

9. Install and configure the GRUB bootloader.

10. Load the installed OS for the first time.
