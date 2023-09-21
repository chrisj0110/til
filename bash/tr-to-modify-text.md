# using tr to modify text

replace `a` with `b`:

```bash
cat file.txt | tr 'a' 'b'
```

to remove all non-digits, use `-c` to select characters not in the set, and `-d` to delete them:

```bash
echo "abc123" | tr -cd '0-9'
```

