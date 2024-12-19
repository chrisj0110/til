# remove newline from copied value

This puts "abc\n" on to the clipboard:

```bash
echo "abc" | pbcopy
```

You can remove newlines like this:

```bash
echo "abc" | tr -d "\n" < /dev/null | pbcopy
```

