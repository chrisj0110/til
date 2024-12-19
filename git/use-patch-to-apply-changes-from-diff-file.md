# use patch to apply changes from .diff file

From the same dir that the diff was taken:

```bash
git apply --ignore-space-change --ignore-whitespace patch.diff
```

via [SO](https://stackoverflow.com/a/15994287/59867)

