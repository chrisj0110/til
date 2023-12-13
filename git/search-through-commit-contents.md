# search through commit contents

To search through the contents of files in history of the current branch:

```bash
git log -i -Sblah
```

`-i` to make it case insensitive.

To do all branches:

```bash
git log -i -Gblah --branches --all
```

Via [SO](https://stackoverflow.com/a/2928721/59867).

