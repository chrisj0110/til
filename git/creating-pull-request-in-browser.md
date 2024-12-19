# creating pull request in browser

After doing a `git push`, you can open a pull request in the browser:

```bash
current_branch=`git branch --show-current | sed -e 's/\//%2F/g'`  # replace / with %2F for URL below
start "https://git.domain.com/projects/project_name/repos/repo_name/pull-requests?create&sourceBranch=refs%2Fheads%2F$current_branch"  # "start" works on windows
```

The reason to do it this way is you can then create .bashrc functions/aliases such that your browser will automatically open the create-pull-request URL when git push is done.

