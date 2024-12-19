# Xargs

Use `xargs` to run a command on each line of output:

```bash
ls *.txt | xargs cat
```

To put each result into its own command (instead of used as params into one command) use `-n 1`:

```bash
xargs -n 1 echo
```

