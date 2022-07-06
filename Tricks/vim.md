# Vim

### Replace string

#### Replce the first occurrence of the string

```
:s/foo/bar/
```

#### Replace all occurrences of the search pattern in the current line

```
:s/foo/bar/g
```

#### Replace the pattern in the entire file

```
:%s/foo/bar/g
```

> `bar` can be empty to remove the string

### move line

```
:m-2 // one line to top
:m+ // one line to button
```

> see forum for set key binding

### Highlight similar words

Just enter `#`

## Source

- [replace string forum](https://stackoverflow.com/questions/19994922/find-and-replace-strings-in-vim-on-multiple-lines)
- [move line forum](https://vi.stackexchange.com/questions/2674/how-can-i-easily-move-a-line?newreg=56ad4fbfe6e24117b82d3b38c0b1a3de)
