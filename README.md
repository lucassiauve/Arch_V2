# Arch_V2
Start from scratch my arch configuration, because my current config is SHIT.

---
# Linux before Windows
Arch must be installed before Windows, because EFI system partition created by Windows is to short for multiple OS (100 MiB). In Addition Windows creates three partitions in a row (Windows Recovery Environment - Microsoft Reserved Partition - Microsoft basic data), so it's more difficult to resize an OS partition when it's between those partitions.
> Arch Wiki [dual-boot Arch-Windows](https://wiki.archlinux.org/title/Dual_boot_with_Windows)

---
# Kernel installation: (Arch)
> Arch Wiki [Installation guide](https://wiki.archlinux.org/title/Installation_guide)

## Partition: (1T SSD)
- EFI system partition -> 1 GiB (with [grub](#Booting) boot loader)
- Swap partition -> 16 GiB
- Linux root partition -> 500 GiB
- Windows root partition -> 483 GiB

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
### Sound system: (Alsa - PipeWire)
- [Alsa](https://wiki.archlinux.org/title/Advanced_Linux_Sound_Architecture) is a [Sound System](https://wiki.archlinux.org/title/Sound_system) that work without any other additional features, the sound card just need to be unmute (be careful, for multiple cards sounds, select the default card and save this in the system config file ```/etc/asound.conf```).
- On top of Alsa, a [Sound servers](https://wiki.archlinux.org/title/Sound_system#Sound_servers) such as [PipeWire](https://wiki.archlinux.org/title/PipeWire) and [PulseAudio](https://wiki.archlinux.org/title/PulseAudio) can offer additional features and support more complex audio configuration (in my case, will be Pipewire). 

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
Install windows OS on the remaining partition, it will detect automatically and use the EFI partition, without creating a new one.

## Time standard
Due to the dual-boot, the Windows clock will be 2h late. To solve this issue, open a powershell with administrator right and run this command:
```
reg add "HKEY_LOCAL_MACHINE\System\CurrentControlSet\Control\TimeZoneInformation" /v RealTimeIsUniversal /d 1 /t REG_DWORD /f
```
If you are having issues with the offset of the time, try reinstalling **tzdata** and then setting your time zone again (in my case Europe/Paris):
```
timedatectl set-timezone Europe/Paris
```
> Arch wiki [System time](https://wiki.archlinux.org/title/System_time#UTC_in_Microsoft_Windows)

## Priority applications
![**LOL**](https://www.leagueoflegends.com/static/logo-1200-589b3ef693ce8a750fa4b4704f1e61f2.png)
