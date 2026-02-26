# reset

if your branch has diverged:

```
On branch my-branch
Your branch and 'origin/my-branch' have diverged,
and have 3 and 82 different commits each, respectively.
  (use "git pull" to merge the remote branch into yours)
```

reset it:

```
git fetch origin
git reset --hard origin/my-branch
```
