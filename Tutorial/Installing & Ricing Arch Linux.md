# Source
- From scratch to having boot menu: [Kskroyal](https://www.youtube.com/watch?v=JRdYSGh-g3s) - From start to 28:25
- [Arch wiki](https://wiki.archlinux.org/title/Installation_guide)
# Preparation
- Download Arch image + Rufus
- Create Bootable usb from Arch Image
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
- Verify efi boot
```shell
ls /sys/firmware/efi/efivars/
```
- Update date & time
```shell
timedatectl status
timedatectl list-timezones
timedatectl set-timezone Asia/Ho_Chi_Minh
```
## Create partition for Arch
- Check partition path
```shell
lsblk
cfdisk /dev/sdax
```
- Create root, home, swap partition -> Write changes
- Format 3 partition one by one
```shell
mkfs.ext4 /dev/sdax
```
- For swap partition
```shell
mkswap /dev/sdax
swapon /dev/sdax
```
- Mount disk to usb boot
```shell
mount /dev/sdax /mnt
mkdir /mnt/home
mount /dev/sdax /mnt/home
lsblk
```
- Setting up fastest mirrors
```bash
cp /etc/pacman.d/mirrorlist /etc/pacman.d/mirrorlist.bak
pacman -Sy
pacman -S pacman-contrib
rankmirrors -n 10 /etc/pacman.d/mirrorlist.bak > /etc/pacman.d/mirrorlist
cat /etc/pacman.d/mirrorlist
```