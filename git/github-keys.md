# Setting up github ssh keys

On a new device:

```bash
ssh-keygen -t ed25519 -C "45946825+chrisj0110@users.noreply.github.com"
eval `ssh-agent`  # make sure this is running
ssh-add ~/.ssh/id_ed25519ssh-add ~/.ssh/
cat ~/.ssh/id_ed25519.pub  # copy the result to the clipboard
```

Navigate to https://github.com/settings/keys and add a new SSH key. Reference the device in the title and paste from the clipboard into Key, and submit.

---

Above comes from https://kinsta.com/blog/generate-ssh-key/
