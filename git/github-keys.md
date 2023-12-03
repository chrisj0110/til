# Setting up github ssh keys

On a new device:

```bash
eval `ssh-agent`  # make sure this is running
```

```bash
export GITHUB_EMAIL=""  # get your github.com email from https://github.com/settings/emails and put it here
```

```bash
ssh-keygen -t ed25519 -C "$GITHUB_EMAIL"
ssh-add ~/.ssh/id_ed25519
cat ~/.ssh/id_ed25519.pub  # copy the result to the clipboard
```

Navigate to https://github.com/settings/keys and add a new SSH key. Reference the device in the title and paste from the clipboard into Key, and submit.

---

Above comes from https://kinsta.com/blog/generate-ssh-key/
