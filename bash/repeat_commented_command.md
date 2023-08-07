# Repeat commented command from history

Comments work on bash commands:

```bash
echo "Hello"  # comment
```

You can use this like a bookmark:

```bash
echo "Imagine some really long but common command here"  # bookmark
```

If you then run N more commands but then want to find the long/common command to run, you can use ctrl-r to find it in history and run it:

```bash
[ctrl-r]# bookmark
```

This works anywhere that comments and ctrl-r work (bash, mysql, etc).

I also posted this at https://unix.stackexchange.com/a/26263/2862
