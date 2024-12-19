# clipboard in windows git bash

To send output to clipboard:

```bash
cat file.txt | clip
```

To get output from clipboard on windows (from within git bash):

```bash
powershell.exe Get-Clipboard > file.txt
```

