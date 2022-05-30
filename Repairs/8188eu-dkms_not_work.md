# 8188eu-dkms not work

1. Remove package
```sh
yay -Rcns 8188eu-dkms
```
2. reboot
3. Install Again
```sh
sudo mhwd -i pci network-r8168
```
4. reboot agin
. *Restart Network Manager if needed*
```sh
sudo systemctl restart NetworkManager
```

[Forum 1](https://archived.forum.manjaro.org/t/r8168-ethernet-why-isnt-this-working/144338/310)
[Forum 2](https://forum.manjaro.org/t/cannot-connect-to-wifi/108019/8)
