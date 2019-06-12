Create bootable USB flash drive

#Linux

  Dd utility

The easiest way. It is recommended to record in this way.

!!! Attention

    This will destroy all data on your USB drive!

!!! Hint

    You can find out the path to the USB device by running the command `lsblk`. Make sure it is not mounted.

```
dd bs = 4M if = / image.iso of = / dev / sd [x]

```
image.iso- the path to the image, `/dev/sd[x]`- the path to the USB device. Use exactly the path `/dev/sdx, not/dev/sdx1`

!!! Attention

    Be careful when specifying a USB device. The utility ddwill not ask questions.
