Download RavanOS to SecureBoot mode

Install SecureBoot

!!! Info

    Installing Astra Linux and subsequent actions should be done only in UEFI mode (ie, with CSM and Legacy modes disabled in BIOS).

For RavanOS SE (OS CH Smolensk) versions 1.5. * - 1.6 and RavanOS CE (OS OH Orel) versions 2.11. * - 2.12, you must install the package astra-safepolicyversion 1.0.32 and higher.

For RavanOS SE (CH Smolensk OS) version 1.5 and RavanOS CE (OH Eagle OS) version 1.11, you must install the packages efitoolsand sbsigntoolthe repository refresh and package astra-safepolicyversion 1.0.32 or higher.

Connect USB flash. In the process, all data on it will be deleted.

Run the command:

    ```sudo astra-secureboot / dev / {usb_flash}```

After executing the command, all the necessary keys will be located in the `/ root / secureboot / key directory`, a bootable USB flash will be created with the necessary files.

Reboot the system. In BIOS (or the F12 function key) select the boot option with UEFI: USB

If everything is done correctly, then KeyTool should load.

In the menu,`KeyToolselectEdit Keys`.

In `it, select db, then Replace Keys`, then your USB device, and then the file `efi / -> boot / -> keys / -> db.auth`.

Repeat the same for first `KEK`, then for `PK`, then go to the main menu by double pressing Esc and select Exit.

After that, reboot, go to BIOS and turn on the mode SecureBoot.

!!! Attention

    With SecureBoot mode enabled, the modes Hibernate and Hybrid-Sleep will not be available.

"Disable SecureBoot"

Recommended shutdown script:

    1. Delete the file `/etc/initramfs/post-update.d/update-efi-image`;

    2. Save a copy of the file `/boot/efi/EFI/astralinux/grubx64.efi`;

    3. Reinstall the grub bootloader.

The sequence of commands:

    'if [-f /etc/initramfs/post-update.d/update-efi-image]; then rm /etc/initramfs/post-update.d/update-efi-image; fi
    mv / boot/efi/EFI/ravanos/grubx64.efi /boot/efi/EFI/ravanos/grubx64.efi-old
    grub-install - bootloader-id = ravanos`
