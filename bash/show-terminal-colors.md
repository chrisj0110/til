# show terminal colors

To show all possible terminal colors:

```bash
for x in {0..255}; do echo -e "\033[38;5;${x}mColor $x\033[0;0m"; done
```

From [here](https://stackoverflow.com/questions/15682537/ansi-color-specific-rgb-sequence-bash#comment132129735_15712766)

To convert RGB colors to ansi 256 colors, [here](https://hm66hd.csb.app/) is one web app that I found from [here](https://gist.github.com/MicahElliott/719710).

Note to self, [dracula color codes](https://github.com/dracula/dracula-theme) map to ansi 256 as follows:

- Background 282a36 => 235
- Cuurent Line / Selection 44475a => 238
- Foreground f8f8f2 => 15
- Comment 6272a4 => 60
- Cyan 8be9fd => 81
- Green 50fa7b => 84
- Orange ffb86c => 215
- Pink ff79c6 => 212
- Purple bd93f9 => 141
- Red ff5555 => 203
- Yellow fafa8c => 228

And some [catppuccin color codes](https://catppuccin.com/) map to ansi 256 as follows:

- Green #a6e3a1 => 151
- Mauve #cba6f7 => 183
- Peach #fab387 => 216
- Pink #f5c2e7 => 225
- Red #f38ba8 => 211
- Sapphire #74c7ec => 81
- SkyBlue #89dceb => 116
- Teal #94e2d5 => 116
- White #cdd6f4 => 189
- Yellow #f9e2af => 223

