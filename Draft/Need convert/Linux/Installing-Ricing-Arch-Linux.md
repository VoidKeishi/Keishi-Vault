# Preparation
- Download Arch image + Rufus

- Create Bootable usb from Arch Image 
	- Rufus setting
		- GPT for UEFI
		- FAT32
		- Cluster 8192 bytes
- Create free space (min 30GB)
- Turn off secure boot, turn on usb boot in BIOS
# Installing
## Setup
- Plug in usb and boot
- Increase font size for better view
```shell
setfont ter-132n
```
- Connect to wifi or LAN
	- ping google.com to check
```shell
iwctl
device list
device [device] show
station [device] get-networks
station [device] connect [wifi]
exit
```
- Update
```shell
pacman -Sy
pacman -Syy
```
- Verify
```shell
pacman -Sy archlinux-keyring
```
## Install using script
- Start script
```shell
pacman -Sy archinstall
archinstall
```
- Config
	- Language
	- Disk
		- Manual
		- btrfs
		- Use compression
	- Boot loader
		- Grub
	- Swap
		- True
	- Root password
	- Add user
	- Profile
	- Network: Use NetworkManager
- Additional packages
```shell
fastfetch htop clang gcc make cmake git curl wget google-chrome
visual-studio-code-bin kitty
```
## GRUB
```shell
sudo pacman -Sy os-prober
sudo nano /etc/default/grub
```
- Change timeout & uncomment "GRUB_DISABLE_OS_PROBER=FALSE"
```shell
sudo grub-mkconfig -o /boot/grub/grub.cfg
```