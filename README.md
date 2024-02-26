# Stuy Linux
The sources for the [Debian Live](https://www.debian.org/devel/debian-live/) based Stuy Linux images.

## Requirements
The [Debian `live-build` toolchain](https://live-team.pages.debian.net/live-manual/html/live-manual/installation.en.html).

Root access (for chroot mechanisms).

~15GiB of free disk space.

## Quickstart
doas lb clean && lb config && doas lb build 2>&1 | tee build.log
