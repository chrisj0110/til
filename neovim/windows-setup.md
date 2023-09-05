# windows setup

On windows the config path is different:

```bash
export NVIM_CONFIG="$HOME/AppData/Local/nvim"
```

To setup NvChad:

```bash
git clone https://github.com/NvChad/NvChad $HOME/AppData/Local/nvim --depth 1 && nvim
```

To setup Vim-Plug:

```bash
curl -fLo $NVIM_CONFIG/site/autoload/plug.vim --create-dirs https://raw.githubusercontent.com/junegunn/vim-plug/master/plug.vim
```

To setup [dracula](https://github.com/Mofiqul/dracula.nvim) theme, add this to `$NVIM_CONFIG/lua/plugins/init.lua`:

```
"Mofiqul/dracula.nvim",
```

..and set it with:

```
colorscheme dracula
```

[Video](https://www.youtube.com/watch?v=4BnVeOUeZxc) to try to setup python tools.

