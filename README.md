# anyfed - Universal Fedora chroot tool

Welcome to anyfed!

An universal Fedora chroot tool which lets you run Fedora anywhere on anything, with or without root.

Version 0.1 (Fedora 24) - https://github.com/nmilosev/anyfed

Supported architectures:
- ARM
- x86_64

This uses a Fedora Docker image to set up a small rootfs somewhere on your system, so that you can chroot into it.

It uses ```chroot``` if you have root, or ```proot``` if you don't.

# Usage

```
wget https://raw.githubusercontent.com/nmilosev/anyfed/master/anyfed && bash anyfed
```

and follow on-screen instructions

# Tested on

- LibreELEC (ARM) - with and without root
- Fedora 24 x86_64 - with and without root
- Ubuntu 16.04 - with and without root
- Arch Linux (2016-09) - with and without root
- Android 6.0 - without root, using Termux (install ```tar``` and ```wget``` first, restart Termux and then run the script)

# GUI applications

You can run GUI applications with ```export DISPLAY=:0``` so they use your host X server. You also have to generate dbus-uuid ```dbus-uuidgen > /etc/machine-id```

# Screenshots

![](https://svbtleusercontent.com/vnfpef68jbt1w_small.png)
![](https://svbtleusercontent.com/h2zz418lnfe7la_small.png)

# License

GPLv3

# Help

Write to me (nmilosev@fedoraproject.org) if you have problems. Have fun! :)
