# vim-surround plugin

The [vim-surround](https://github.com/tpope/vim-surround) plugin also supports putting quotes around a visual block:

```
test
```

with the word `test` in a visual block, then command `S"`, to end up with:

```
"test"
```

then with cursor inside the quotes above you can do `cs"'` to change it to single quotes.

