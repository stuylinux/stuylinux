# Stuy Linux
The sources for the [Debian Live](https://www.debian.org/devel/debian-live/) based Stuy Linux images.

## Requirements
The [Debian `live-build` toolchain](https://live-team.pages.debian.net/live-manual/html/live-manual/installation.en.html).

Root access (for chroot mechanisms).

~15GiB of free disk space.

## Quickstart
```
lb clean
lb config
doas lb build 2>&1 | tee build.log
```

## NetLogo
As of right now, the NetLogo .deb package is built through manually patching the
release binaries with an installer Makefile, along with an XDG desktop file.

Build recipes can be found at https://git.stuylinux.org/stuylinux/netlogo-deb.

The generated `netlogo_6.4.0-1_all.deb` should be copied into `config/packages.chroot/`.
