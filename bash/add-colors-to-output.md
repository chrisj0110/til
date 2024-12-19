# add colors to output

to change the letter b to blue:

```bash
export blue=$'\033[38;2;137;180;250m'
export clear=$'\033[0m'
echo "abc" | sed -E "s/([a-z])([a-z])([a-z])/\1${blue}\2${clear}\3/g"
```

Note: to convert RGB to ansi color is basically f"\033[38;2;{r};{g};{b}m"

