# setting upstream on push

If you get an error when pushing to a newly-cloned repo that looks like: "The current branch ... has no upstream branch.", then:

```bash
git config --global push.autoSetupRemote true
```

from [SO](https://stackoverflow.com/a/23402125)

