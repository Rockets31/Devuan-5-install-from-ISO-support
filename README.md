# Devuan-5-install-from-ISO-support
Directly boot & install Devuan-5 from Official Devuan Installation Media using grub2 without burning to usb-drive.

# Features
- Filesystems: exfat, ext4
- Provide devuan boot menu
- Supported ISOs: Devuan-desktop, Devuan-netinst & Devuan-server of Devuan-5 release.

# Usage
Load provided 'scandev-daedalus.gz' along with the main 'initrd' of the installation media via grub loopback module.
If you are using 'https://github.com/Mexit/MultiOS-USB', it is just a few steps:

0. Use MultiOS-USB partition on 'exfat' or 'ext4' filesystem.
1. Copy your Devuan-5-iso files to 'ISOs' directory.
2. Create a directory for 'grub.cfg' files: '/MultiOS-USB/config_priv/devuan-scandev'
3. Copy 'scandev-daedalus.gz' & 'devuan-daedalus-desktop.cfg' over there.
4. Reboot into 'MultiOS-USB' and start e.g. 'devuan_daedalus_5.0.1_amd64_desktop.iso [scandev]' entry.
5. Installer will start same way as from usb-stick.
