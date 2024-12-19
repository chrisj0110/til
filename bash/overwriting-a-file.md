# overwriting a file

in order to modify the contents of a file and write it back:

```bash
contents=$(cat file) && echo "$contents" | some-command > file
```

