# Xargs

Use `xargs` to run a command on each line of output:

```bash
ls *.txt | xargs -I {} cat {}
```
