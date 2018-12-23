# manjaro-arm-installer

[WIP] Scripts for installing Manjaro ARM directly to SD/eMMC cards without the need for images.

This script is "interactive". Meaning that it asks you questions when run to customize your install. Like username, password etc.


## Dependencies:
* bash
* wget
* git
* systemd
* dialog
* parted
* libarchive

## Installing:
To use this script, please make sure that the following is correct:

* an SD card with at least 4 GB storage is plugged in.

## Known Issues:
* none

## Usage:
To use this script, simple run it as normal user after you make it executable:
```
chmod +x manjaro-arm-installer
bash /manjaro-arm-installer
```

## Other notes:
This script will soon by available as a **Arch** (*pkg.tar.xz*) package in my **Manjaro Strit** repo.

This script **should** be distro-agnostic, which means you can install *Manjaro ARM* from **any** distro, as long as the dependencies are met.
