# Pacman

### Browsing packages

```sh
pacman -Qq | fzf --preview 'pacman -Qil {}' --layout=reverse --bind 'enter:execute(pacman -Qil {} | less)'
```

### Removing unused packages [orphans]

Orphans are packages that were installed as a dependency and are no longer required by any package.

```zsh
pacman -Qtdq | pacman -Rns -
```

> If no orphans were found, the output is error: argument '-' specified with empty stdin. This is expected as no arguments were passed to pacman -Rns.

## Source

- [browsing packages](https://wiki.archlinux.org/title/pacman/Tips_and_tricks#Listing_packages)
- [Removing unused packages](<https://wiki.archlinux.org/title/pacman/Tips_and_tricks#Removing_unused_packages_(orphans)>)
