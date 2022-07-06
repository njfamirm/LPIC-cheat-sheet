# Git

### Fetch remote branch

```sh
git branch -r
git checkout -b x origin/x
```

or easier...

```sh
git checkout --track origin/<REMOTE_BRANCH_NAME>
```

### Run bash script in .gitconfig

```
test="!command"
```

### Remove tracking branches no longer on remote

```sh
git fetch -p && for branch in $(git for-each-ref --format '%(refname) %(upstream:track)' refs/heads | awk '$2 == "[gone]" {sub("refs/heads/", "", $1); print $1}'); do git branch -D $branch; done
```

## Source

- [fetch remote branch forum1](https://stackoverflow.com/a/10313379/18004491)
- [fetch remote branch forum2](https://stackoverflow.com/a/60210807/18004491)
- [run bash script in .gitconfig forum](https://stackoverflow.com/a/14994923/18004491)
- [remove tracking branches no longer on remote](https://stackoverflow.com/a/33548037/18004491)
