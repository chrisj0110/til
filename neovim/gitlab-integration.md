# gitlab integration

first, use [vim-fugitive](https://github.com/tpope/vim-fugitive):

```lua
use("tpope/vim-fugitive")
```

then use [fugitive-gitlab](https://github.com/shumphrey/fugitive-gitlab.vim):

```lua
use("shumphrey/fugitive-gitlab.vim")
```

and configure it:

```lua
vim.g.fugitive_gitlab_domains = {'gitlab.domain.com'}
```

