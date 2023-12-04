# pass a command from the command line

use `-c` to pass a command to vim. For example, to run ripgrep through fzf.vim:

```bash
vim -c ":Rg"
```

Multiple commands can be separated by `|`.

