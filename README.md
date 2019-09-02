# anyfed - Universal Fedora chroot tool

Welcome to anyfed!

An universal Fedora chroot tool which lets you run Fedora anywhere on anything, with or without root.

Supported architectures:
- ARM64 (aarch64)
- x86_64
- ARM32 (armhfp) - from Docker Hub

This uses a Fedora Docker image to set up a small rootfs somewhere on your system, so that you can chroot into it.

It uses ```chroot``` if you have root, or ```proot``` if you don't.

# Usage

```
wget https://raw.githubusercontent.com/nmilosev/anyfed/master/anyfed && bash anyfed
```

For Termux (Android):

```apt update && apt install tar wget -y && export PATH=$PATH && wget https://raw.githubusercontent.com/nmilosev/anyfed/master/anyfed && bash anyfed```

and follow on-screen instructions

# Tested on

- LibreELEC (ARM) - with and without root
- OpenELEC (ARM) - with and without root
- Fedora 24 x86_64 - with and without root
- Ubuntu 16.04 - with and without root
- Arch Linux (2016-09) - with and without root
- Android 6.0 - without root, using Termux (see instructions above)

# GUI applications

You can run GUI applications with ```export DISPLAY=:0``` so they use your host X server. You also have to generate dbus-uuid ```dbus-uuidgen > /etc/machine-id```

You also may need ```xhost +``` on your host system.

# Screenshots

![](https://svbtleusercontent.com/vnfpef68jbt1w_small.png)
![](https://svbtleusercontent.com/h2zz418lnfe7la_small.png)

# License

GPLv3

# Help

Write to me (nmilosev@fedoraproject.org) if you have problems. Have fun! :)
