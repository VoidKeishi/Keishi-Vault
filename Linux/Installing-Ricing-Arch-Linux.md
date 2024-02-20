# Source
- From scratch to having boot menu: [Kskroyal](https://www.youtube.com/watch?v=JRdYSGh-g3s) - From start to 28:25
- [Arch wiki](https://wiki.archlinux.org/title/Installation_guide)
- https://wiki.archlinux.org/title/General_recommendations
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
## Install basic packages
- Setting up fastest mirrors
```bash
cp /etc/pacman.d/mirrorlist /etc/pacman.d/mirrorlist.bak
pacman -Sy
pacman -S pacman-contrib
rankmirrors -n 10 /etc/pacman.d/mirrorlist.bak > /etc/pacman.d/mirrorlist
cat /etc/pacman.d/mirrorlist
```
- Install packages
```shell
pacstrap -i /mnt base base-devel linux linux-lts linux-headers linux-firmware intel-ucode sudo nano vim neofetch networkmanager dhcpcd pulseaudio
```
## Generate FSTAB
```shell
genfstab -U /mnt >> /mnt/etc/fstab
cat /mnt/etc/fstab
```
## Chroot to new system
```shell
arch-chroot /mnt
lsblk
```
## Config root and user account
```shell
passwd
useradd -m void_keishi
passwd void_keishi
usermod -aG wheel,storage,power void_keishi
nano visudo
```
- Uncomment "%wheel ALL=(ALL)"
- Add "Defaults timestamp_timeout=0"
- Config language
```shell
nano /etc/locale.gen
locale-gen
echo LANG=en_US.UTF-8 > /etc/locale.conf
export LANG=en_US.UTF-8
```
## Setup hostname
```shell
echo ArchLinux > /etc/hostname
nano /etc/hosts
127.0.0.1 localhost
::1 localhost
127.0.1.1 ArchLinux.localdomain localhost
```
## Setting timezone, region
```shell
ln -sf /usr/share/zoneinfo/Asia/Ho_Chi_Minh /etc/localtime
hwclock --systohc
```
## GRUB
```shell
mkdir /boot/efi
mount /dev/sda1 /boot/efi/
pacman -S grub efibootmgr dosftools mtools
nano /etc/default/grub
```
- Uncomment GRUB_DISABLE_OS_PROBER=false
- Mount the EFI system
```shell
pacman -S os-prober
grub-install --target=x86_64-efi --bootloader-id=grub_uefi --recheck
grub-mkconfig -o /boot/grub/grub.cfg
ls /boot/efi/EFI/
ls /boot/efi/EFI/grub_uefi/
systemctl enable dhcpcd.service
systemctl enable NetworkManager.service
umount -lR /mnt
reboot
```
# Ricing
## Desktop GUI
### Desktop manager
- SDDM
- GDM
- LightDM
### Window managers
- bspwm
- i3
- icewm
- qtile
### Compositor
- picom
### Desktop enviroment (dont need)
## Utility
- rofi
- polybar
- alacritty
- feh
- neofetch
- zsh
- Ibusbamboo