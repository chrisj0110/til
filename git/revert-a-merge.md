# revert a merge

List recent merges: 

```bash
git log --merges --oneline
```

copy the hash you want and:

```bash
git revert -m 1 [hash]
```

