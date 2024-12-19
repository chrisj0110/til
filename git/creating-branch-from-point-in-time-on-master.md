# creating branch from point in time on master

```bash
git checkout -b new-branch-name `git rev-list -n 1 --before="1 week ago" master`
```

