# remove history

to remove all history from a git repo and start over:

```bash
rm -rf .git
git init
git add .
git commit -m "rewrite history"
git remote add origin [repo-url]
git push --force --set-upstream origin main
```

