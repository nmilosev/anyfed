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
wget https://raw.githubusercontent.com/nmilosev/anyfed/master/anyfed && chmod +x anyfed && ./anyfed
```

and follow on-screen instructions

# License

GPLv3

# Help

Write to me (nmilosev@fedoraproject.org) if you have problems. Have fun! :)