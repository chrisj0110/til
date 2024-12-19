# fzf

See [here](https://github.com/junegunn/fzf)

notes:

- `**<tab>` to find files, or just `ctrl-t`
- `| fzf` - pipe some output to fzf to select value(s)
  - `| fzf --multi` or `-m` to select multiple values
- `ctrl-j` and `ctrl-k` to move cursor up and down
- `|` is an or operator
- `tab` and `shift-tab` to select/unselect multiple items
- `ctrl-x` in vim to open the result in a new horizontal split

vim info [here](https://github.com/junegunn/fzf/blob/master/README-VIM.md) and [here](https://github.com/junegunn/fzf.vim)

Example of using fzf to select value(s):

```bash
$ echo "one
two
three
" | fzf --multi | xargs -n 1 echo
```

