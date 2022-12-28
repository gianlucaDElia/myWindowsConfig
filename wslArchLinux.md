# WSL Acrh linux configuration
Download [Arc](https://github.com/yuk7/ArchWSL), extract it on C:/ArchLinux and run the exe. Run the exe two times.

Change root password
```
passwd
```

Config keys and update
```
pacman-key --init
pacman-key --populate
pacman -Sy archlinux-keyring
pacman -Su
```

Add user
```
useradd -m -G wheel,audio,video,storage -s /bin/bash gian
passwd gian
EDITOR=vim visudo
```

Set default user
```
./Arch.exe config --default-user gian
```

Install base-devel and general packages
```
pacman -S base-devel git cmake ninja wget zip unzip
```
if error of fakeroot-tcp
```
pacman -R fakeroot-tcp
```
