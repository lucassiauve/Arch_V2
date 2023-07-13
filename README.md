# Arch_V2
Start from scratch my arch configuration, because my current config is SHIT.

---
# Dual-boot: (Arch - Windows11)
Arch must be installed before Windows, because EFI system partition created by Windows is to short for multiple OS (100 MiB). In Addition Windows creates three partitions in a row (Windows Recovery Environment - Microsoft Reserved Partition - Microsoft basic data), so it's more difficult to resize an OS partition when it's between those partitions.
> Arch Wiki for [dual-boot Arch-Windows](https://wiki.archlinux.org/title/Dual_boot_with_Windows)

---
# Kernel installation: (Arch)
> Arch Wiki [Installation guide](https://wiki.archlinux.org/title/Installation_guide)

## Partition: (1T SSD)
- EFI system partition -> 1 GiB (with grub boot loader)
- Swap partition -> 16 GiB
- root partition -> 983 GiB (

## Swap end ZRam

## Systemd

## Environment variables

---
# Post installation

## System administration

## Package management: (Pacman->Yay)

## Booting
### Boot loader: (Grub)
### Dual boot: (Windows)

## Graphical interface
### Windows Manager: (Sway)
Update: https://github.com/swaywm/sway/releases
Source Code: https://github.com/swaywm/sway
Wiki: https://github.com/swaywm/sway/wiki
Chat: https://web.libera.chat/gamja/?channels=#sway

## Power management

## Multimedia
### Sound system: (PipeWire)

## Networking

## Input devices

## System services

## Appearance
### Font: (Source Code Pro SemiBold)
### GTK theme

## Console improvement
### Shell: (FISH)
### Shell Emulator: (Alacritty)
### Windows Switcher | Ssh-launcher | Run Dialog | dmenu: (ROFI)
### Neovim

---
# Additional applications

---
# Windows installation: (Windows 11)

## Priority applications
![**LOL**](https://www.leagueoflegends.com/static/logo-1200-589b3ef693ce8a750fa4b4704f1e61f2.png)
