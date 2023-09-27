# show terminal colors

To show all possible terminal colors:

```bash
for x in {0..255}; do echo -e "\033[38;5;${x}mColor $x\033[0;0m"; done
```

From [here](https://stackoverflow.com/questions/15682537/ansi-color-specific-rgb-sequence-bash#comment132129735_15712766)

