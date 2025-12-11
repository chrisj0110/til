# pull in changes from another branch

If I committed changes in branch-a and want to pull them into branch-b, I can checkout branch-b and do:

```bash
git checkout --patch branch-a
```

this will ask me which changes I want to pull in from branch-a into branch-b

Or to pull in changes as local modifications instead of committing:

```bash
git merge --no-commit branch-a
```
