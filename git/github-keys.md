# Setting up github ssh keys

On a new device:

```bash
# make sure this is running:
eval `ssh-agent`
```

```bash
# if not already set, get your github.com email from https://github.com/settings/emails and put it here
export GITHUB_EMAIL=""
```

NOTE: if having issues on a machine that used to work, try adding something like this to ~/.ssh/config:

```
Host github.com
  Hostname github.com
  User git
  IdentityFile ~/.ssh/id_ed25519_github1
```

```bash
ls -l ~/.ssh/id_ed25519_github?
# bump the number if it already exists:
export GH_FILE_NAME="~/.ssh/id_ed25519_github1"
echo $GH_FILE_NAME | pbcopy
# paste the value from clipboard when prompted after running this command:
ssh-keygen -t ed25519 -C "$GITHUB_EMAIL"
ssh-add $GH_FILE_NAME
cat $GH_FILE_NAME.pub | pbcopy
```

Navigate to https://github.com/settings/keys and add a new SSH key. Reference the device in the title and paste from the clipboard into Key, and submit.

---

Above initially came from https://kinsta.com/blog/generate-ssh-key/

