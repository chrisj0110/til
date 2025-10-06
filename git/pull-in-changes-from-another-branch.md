# pull in changes from another branch

If I committed changes in branch-a and want to pull them into branch-b, I can do:

```bash
git diff origin/master..branch-a > /tmp/a.patch && git apply --3way --index /tmp/a.patch
```

this will pull in changes from branch-a into branch-b as staged changes, then I can choose which changes to commit.

