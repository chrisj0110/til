# setup

See video from [ThePrimagen](https://www.youtube.com/watch?v=w7i4amO_zaE). More notes below:

I was successful on windows using ~/AppData/Local/nvim for my configuration. So the clone command for packer is `git clone --depth 1 https://github.com/wbthomason/packer.nvim ~/AppData/Local/nvim/pack/packer/start/packer.nvim`.

When adding a new plugin, add it to packer.lua, do `:so` then `:PackerSync`.

Treesitter will error on `help` - you can remove it or find a replacement for it.

Treesitter will need a C compiler installed and in the path. See [zig](https://ziglang.org/download/) for windows. Unzip it into a folder and add that folder to PATH.


