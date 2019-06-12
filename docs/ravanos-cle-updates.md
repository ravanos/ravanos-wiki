RavanOS CLE can update from the public network repository.

The default repository url is below:

```
https://download.ravanos.org/cle/current/repository/
```

In cases where the standard network repository for any reason is not possible to use, you can apply to perform an update from removable media or create your own repository.

If you can not access the network repository for some reason, you can perform <updates from removable media> or <create your own repository>

Before performing an OS update, update the local repository cache first. This can be done with the `Update` button in the graphical package manager, or from the command line with the command:

```
sudo apt update
```

After the system updates list completed, yoyu can check the list of packages with updated versions by executing the following command.

```
apt list-upgradable
```

Finally you can execute the following command to install the  updates.

```
sudo apt dist-upgrade
```

!!! Warning

    Using the command `sudo apt upgrade`  is not recommended, as this command performs less installation checks.

!!! Info

    After completing the update, it is recommended to reboot the system
