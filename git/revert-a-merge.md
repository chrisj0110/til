# revert a merge

List recent merges: 

```bash
git log --merges --oneline
```

copy the hash you want and:

```bash
git revert -m 1 [hash]
```

to keep it (as staged) without committing:

```bash
git diff <hash>^ <hash> | git apply -R
```
