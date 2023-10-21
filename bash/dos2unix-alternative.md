# dos2unix alternative for line endings

If `dos2unix` is not available, this works:

```bash
sed -i 's/\r$//' file
```

Or recursively:

```bash
find directory -type f -print0 | xargs -0 sed -i 's/\r$//'
```

