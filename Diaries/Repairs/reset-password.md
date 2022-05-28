# Reset password

### Change user password

1. mount and chroot to local shell from live boot
2. change password
```sh
passwd root
passwd USER
```

but kwallet password does not change!

### Change kwallet password

1. Install KwalletManager
2. Change password!

### Reset kwallet password

It is not possible to recover the password when you forget the password
and you must delete the previous ones completely!

```sh
cd $HOME/.local/share/kwalletd/ 
BACKUP_DATE=$(date +"%F-%X")
mv kdewallet.kwl "kdewallet.kwl-${BACKUP_DATE}.bak"
mv kdewallet.salt "kdewallet.salt-${BACKUP_DATE}.bak"
```

## Source

- [reset kwallet password forum](https://unix.stackexchange.com/a/578403)

