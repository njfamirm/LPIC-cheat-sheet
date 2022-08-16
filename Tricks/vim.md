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

Use `#`

### Go to end of line

Use `$`

### Move between word

Use `b` to move back one word.

Use `w` to move forward one word.

## Source

- [replace string blog](https://linuxize.com/post/vim-find-replace/#:~:text=quick%20and%20easy.-,Basic%20Find%20and%20Replace,press%20the%20'Esc'%20key.)
- [move line forum](https://vi.stackexchange.com/questions/2674/how-can-i-easily-move-a-line?newreg=56ad4fbfe6e24117b82d3b38c0b1a3de)
- [go to end of line forum](https://stackoverflow.com/a/105734/18004491)
