# Pip list available versions

To list available versions of a package:

```bash
pip index versions packagename
```

To get the comma-separated values on to their own lines:

```bash
pip index versions packagename | grep "Available versions" | awk -F": " '{print $2}' | sed -e "s/, /\n/g"
```
