# Updating and switching to master

Normally I would:

```bash
git checkout master
git pull
```

This causes your code to potentially change twice: 1) switching from your branch to master, and 2) updating master. Things like your VSCode python language server and plugins might have to deal with 2 code changes (A => B => C).

This can instead be done with just one change:

```bash
git fetch origin master:master  # update your master branch even though it's not checked out
get checkout master
```

Now your code only changes once, during the second step. (A => B)
