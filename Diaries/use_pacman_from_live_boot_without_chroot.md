`/usr/lib/libc.so.6: version `GLIBC_2.34’ not found`

https://bbs.archlinux.org/viewtopic.php?id=274705
https://wiki.archlinux.org/title/Pacman#Pacman_crashes_during_an_upgrade

1- mount root
2- mount -t proc proc /mnt/proc
3- mount --rbind /sys /mnt/sys
4- mount --rbind /dev /mnt/dev

```
pacman --sysroot /mnt
```

for example pacman --sysroot /mnt -S gcc
