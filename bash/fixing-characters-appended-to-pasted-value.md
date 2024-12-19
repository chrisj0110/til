# fixing characters appended to pasted value

Sometimes in my windows git bash window a value like `1~` is appended to a value that I paste, as reported [here](https://github.com/microsoft/vscode/issues/141879).

[This](https://askubuntu.com/a/738649) seems to fix it: `bind 'set enable-bracketed-paste off'`

