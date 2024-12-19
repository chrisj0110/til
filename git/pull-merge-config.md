# git pull merge config

If you do `git pull` and get a hint that starts with `Pulling without specifying how to reconcile divergent branches is discouraged`, you can update your global setting:

```bash
git config --global pull.rebase false
```

