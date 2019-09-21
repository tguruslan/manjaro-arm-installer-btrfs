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
* debian-whois-mkpasswd
* gawk

## Installing and using from gitlab:
To use this script, please make sure that the following is correct:

* an **empty** SD/eMMC card with at least 8 GB storage is plugged in.
* that your user account has `sudo` rights.

Then use this to get it:
```
git clone https://gitlab.manjaro.org/manjaro-arm/applications/manjaro-arm-installer
cd manjaro-arm-installer
chmod +x manjaro-arm-installer
sudo -s
clear && bash manjaro-arm-installer
```

## Known Issues:
* Because `dialog` is weird, the script needs to be run in `bash`.

## Supported Devices:
* Pinebook
* Raspberry Pi 3B
* raspberry Pi 4 (new)
* Rock64
* RockPro64
* Odroid C2
* Odroid N2
* Khadas Vim 3 (new)
* Rock Pi 4
* Pine64-LTS / Sopine
* Pine64+
* Khadas Vim 1 (new)

## Supported Editions / Desktops:
* Minimal (no xorg, no apps)
* KDE/Plasma (full plasma desktop with apps)
* XFCE (full XFCE desktop with apps)
* LXQT (full LXQT desktop with some qt apps)
* Mate (full mate desktop with apps)
* CuboCore (base plasma desktop with CoreApps)

## Other notes:
This script is available in the **Manjaro** repository and can be installed with `sudo pacman -S manjaro-arm-installer`.

This script is also available as an **Arch** (*pkg.tar.xz*) package in my **Manjaro Strit** repo, called `manjaro-arm-installer`.

This script **should** be distro-agnostic, which means you can install *Manjaro ARM* from **any** distro, as long as the dependencies are met.
