# Viewing only files changed in a commit

To just list the files changed in a commit with hash abc123:

```bash
git diff --name-only abc123^..abc123
```

To make a kind of alias to where you don't have to put the commit hash twice:

```
function gdf() {
    git diff --name-only $1^..$1
}
```

and call it like:

```bash
gdf abc123
```
