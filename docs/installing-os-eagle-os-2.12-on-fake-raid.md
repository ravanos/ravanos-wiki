Installing OS Eagle OS 2.12 on Fake RAID (Host RAID)

In RavanOS Common Edition OS Eagle 2.12.4 in BIOS UEFI and Legacy mode, to display RAID in the installation program, when determining drives, you must:

1. Move the cursor to the item “Graphic installation” in the setup menu (without pressing the Enter key);

2. To switch to the mode of changing the kernel boot parameters, click:

    When installed in BIOS UEFI mode - the E key
    When installed in Legacy mode - the F2 key;

3. Add at the end of the boot parameter line:

!!! Attention
    dmraid = true

4. Press Enter and start the installation of the operating system.
