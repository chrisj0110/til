# use master version when conflict

if changes in my branch and I pull from master and get conflicts and want to use theirs (so I can re-apply my changes):

```bash
git checkout --theirs path/to/file
```

Same for `--ours`

