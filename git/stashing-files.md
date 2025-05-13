# stashing files

To stash just one file: `git stash -- filename.txt`

To stash one file with a message: `git stash push -m "describe changes to filename.ext" filename.ext`

To stash all staged files with a message: `git stash push -m "describe changes"`

To interactively select hunks to put on the stash: `git stash push -p -m "message"`

To view a diff of a stash:

```bash
git stash show -p stash@{0}  # replace the number
```

To delete the most-recent stash: `git stash drop`
