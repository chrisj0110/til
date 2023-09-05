# list extensions

To list the installed extensions (into a new file):

```bash
code --list-extensions > installed-extensions.txt
```

If you have a fresh VSCode install and a list of desired extensions, you can install them:

```bash
while read line; do code --install-extension "$line"; done < installed-extensions.txt
```

