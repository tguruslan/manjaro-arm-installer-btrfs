# manjaro-arm-installer-btrfs

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
* openssl
* gawk
* dosfstools
* polkit

## Installing and using from git:
To use this script, please make sure that the following is correct:

* an **empty** SD/eMMC card with at least 8 GB storage is plugged in, but not mounted.
* that your user account has `sudo` rights.

Then use this to get it:
```
git clone https://github.com/tguruslan/manjaro-arm-installer-btrfs
cd manjaro-arm-installer
chmod +x manjaro-arm-installer
sudo bash ./manjaro-arm-installer
```

## Known Issues:
* Because `dialog` is weird, the script needs to be run in `bash`.

## Supported Devices:
* Raspberry Pi 4
* Raspberry Pi 3B
* Pinebook Pro
* RockPro64
* Rock Pi 4
* Odroid N2
* Odroid C4 (new)
* Odroid C2
* Pinebook
* Pine64-LTS / Sopine
* Pine64+
* Pine H64 (new)
* Rock64
* LibreComputer Renegade (new)
* Khadas Vim 3
* Khadas Vim 2
* Khadas Vim 1

## Supported Editions / Desktops:
* Minimal (no xorg, no apps)
* KDE/Plasma (full plasma desktop with apps)
* XFCE (full XFCE desktop with apps)
* i3 (tiling window manager with gtk apps)
* LXQT (full LXQT desktop with some qt apps)
* Mate (full mate desktop with apps)
* CuboCore (base plasma desktop with CoreApps)
