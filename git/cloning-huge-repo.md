# Cloning huge repo

If a repo is too big to clone, you can do this (replace "url"):

```bash
git clone --filter=blob:none url
```

Git will then only download the contents of a file when needed, rather than downloading the contents of the entire history up front.
