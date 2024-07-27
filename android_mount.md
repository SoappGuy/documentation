# Mount media transfer protocol (MTP) devices (android phones)

### Manual mount
```sh
paru -S gvfs-mtp

# list devices
gio mount -li | grep activation_root

# mount device by path
gio mount 'path'

# device will be mounted at
ls /run/user/1000/gvfs
```

### Auto mount
Just install:
* mtpfs → for media transfer protocol
* jmtpfs → for later version supports
* gvfs-mtp → for auto mount MTP
* gvfs-gphoto2 → for auto mount PTP

```sh
paru -S mtpfs, jmtpfs, gvfs-mtp, gvfs-gphoto2
```
