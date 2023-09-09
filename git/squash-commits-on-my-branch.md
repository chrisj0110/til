# Squash commits on my branch

If you have, for example, 4 commits you want to squash together, then:

```bash
export BRANCH=""  # fill this in with feature/branch-name, whatever it is
```

```bash
git rebase -i origin/$BRANCH~4 $BRANCH  # replace the 4 with the number of most-recent commits
```

```bash
# you'll get prompted here: select "squash" for the top ones, and "pick" for the bottom one
# then you'll get prompted for the commit message - you can leave the default, or change it
git push origin +$BRANCH
```

More details [here](https://stackoverflow.com/a/5668050/59867)

