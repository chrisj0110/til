# Squash commits on my branch

NOTE: to edit commits, see [SO](https://stackoverflow.com/a/3042512/59867). To edit the first commit, start with `git rebase -i --root`, then `edit` for the first one, then make the chnage, commit, then `git rebase --continue`. `git push -f` to force the push.

If you have, for example, 4 commits you want to squash together, then:

```bash
export BRANCH=""  # fill this in with feature/branch-name, whatever it is
```

```bash
git rebase -i origin/${BRANCH}~4 $BRANCH  # replace the 4 with the number of most-recent commits
```
You'll get prompted here: select "squash" for the top ones, and "pick" for the bottom one then you'll get prompted for the commit message - you can leave the default, or change it

```bash
git push origin +$BRANCH
```

More details [here](https://stackoverflow.com/a/5668050/59867)
Video on `git rebase --interactive` [here](https://www.youtube.com/watch?v=H7RFt0Pxxp8)

