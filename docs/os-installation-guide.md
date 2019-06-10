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
