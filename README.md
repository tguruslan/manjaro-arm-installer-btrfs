# manjaro-arm-installer

Scripts for installing Manjaro ARM directly to SD/eMMC cards without the need for images.

This script is "interactive". Meaning that it asks you questions when run to customize your install. Like username, password etc.


## Dependencies (Arch package names):
* bash
* wget
* git
* systemd
* dialog
* parted
* libarchive
* binfmt-qemu-static
* mkpasswd
* gawk

## Installing:
To use this script, please make sure that the following is correct:

* an SD/eMMC card with at least 8 GB storage is plugged in (but not mounted).
* that your user account has `sudo` rights.

## Known Issues:
* Because `dialog` is weird, the script needs to be run in `bash`.

## Usage:
To use this script, simple run it as normal user after you make it executable:

```
chmod +x manjaro-arm-installer
sudo -s
clear && bash manjaro-arm-installer
```

## Other notes:
This script is available as a **Arch** (*pkg.tar.xz*) package in my **Manjaro Strit** repo, called `manjaro-arm-installer`.

This script **should** be distro-agnostic, which means you can install *Manjaro ARM* from **any** distro, as long as the dependencies are met.
