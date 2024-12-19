# Using sed to just print a certain line of output

If you want to filter down to just the second line of multiple lines of output, you can do:

```bash
$ echo "one
> two
> three" | sed -n "2p"
```

This outputs `two`.

`-n` is to suppress sed automatically printing every line of output.

`2` specifies the line number.

`p` tells sed to print the current line.
