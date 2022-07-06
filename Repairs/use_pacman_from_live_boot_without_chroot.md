# Use pacman from live boot without chroot

log

```sh
/usr/lib/libc.so.6: version `GLIBC_2.34’ not found
```

1. mount root
2. mount -t proc proc /mnt/proc
3. mount --rbind /sys /mnt/sys
4. mount --rbind /dev /mnt/dev
5. Install package

```sh
pacman --sysroot /mnt PACKAGE_NAME
```

## Source

- [Forum](https://bbs.archlinux.org/viewtopic.php?id=274705)
- [Doc](https://wiki.archlinux.org/title/Pacman#Pacman_crashes_during_an_upgrade)
