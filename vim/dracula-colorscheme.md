# Dracula colorscheme

On a new device:

```bash
mkdir -p ~/.vim/pack/themes/start
cd ~/.vim/pack/themes/start
git clone https://github.com/dracula/vim.git dracula
```

From [here](https://draculatheme.com/vim)

For Dracula Pro:

Copy the themes/vim folder from the zip file and rename it:

```bash
cp -r vim ~/.vim/pack/themes/start/dracula_pro
```

And enable dracula pro in vimrc.

Note: GCP Cloud Shell defaults the number of colors to `t_Co=8`. Changing it using `set t_Co=256` fixes the colorscheme.

