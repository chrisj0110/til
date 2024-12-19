# Settings

Some settings I use:

```json
{
    // performance
    "files.exclude": {
        "**/__pycache__": true,
        "**/.mypy_cache": true,
        "**/.pytest_cache": true,
    },
    "search.exclude": {
        "**/site-packages/**": true,
    },
    "editor.minimap.enabled": false,
    "search.searchOnType": false,
    "editor.codeLens": false,

    "editor.minimap.renderCharacters": false, // https://www.reddit.com/r/vscode/comments/hrorvc/tip_disable_editorminimaprendercharacters/
    "editor.acceptSuggestionOnEnter": "off", // https://www.reddit.com/r/vscode/comments/ayvd0p/how_to_stop_autocomplete_with_enter/
    "editor.snippetSuggestions": "inline", // https://stackoverflow.com/a/42107910/59867 https://code.visualstudio.com/docs/editor/intellisense#_customizing-intellisense
    "editor.rulers": [
        160
    ],
    "workbench.colorTheme": "Dracula",
    "workbench.colorCustomizations": {
        "[Dracula]": {
            "tab.activeBorderTop": "#0A84FF", // Active Tab Top Highlighting
            "editor.background": "#282A36" // change this to the dracula pro background that I like
        }
    },
    "vim.normalModeKeyBindingsNonRecursive": [
        {
            "before": [
                ":",
                "W"
            ],
            "after": [
                ":",
                "w"
            ]
        },
        {
            "before": [
                ":",
                "Q"
            ],
            "after": [
                ":",
                "q"
            ]
        }
    ],
    "vim.handleKeys": {
        "<C-a>": false,
        "<C-c>": false,
        "<C-g>": false,
        "<C-o>": false,
        "<C-w>": false,
        "<C-y>": false,
        "<C-pageup>": false,
        "<C-pagedown>": false,
    },
    "vim.visualModeKeyBindings": [
        {
            "before": [
                ">"
            ],
            "commands": [
                "editor.action.indentLines"
            ]
        },
        {
            "before": [
                "<"
            ],
            "commands": [
                "editor.action.outdentLines"
            ]
        },
    ],
    "vim.foldfix": true,
    "python.languageServer": "Pylance",
    "[python]": {
        "editor.formatOnType": true,
        "editor.codeActionsOnSave": {
            "source.organizeImports": true
        },
        "editor.defaultFormatter": "ms-python.black-formatter",
        "editor.formatOnSave": true,
    },
    "black-formatter.args": [
        "--line-length",
        "160"
    ],
    "search.exclude": {
        "**/site-packages/**": true,
    },
    "gitlens.integrations.enabled": true,
    "workbench.tree.indent": 24,
    "workbench.sideBar.location": "right",
    "workbench.editor.limit.enabled": true,
    "editor.formatOnSave": true,
    "jupyter.experiments.enabled": false,
    "jupyter.interactiveWindow.creationMode": "single",
    "jupyter.interactiveWindow.viewColumn": "active",
    "terminal.integrated.copyOnSelection": true,
    "terminal.integrated.rightClickBehavior": "paste",
    "terminal.integrated.commandsToSkipShell": [
        "workbench.action.toggleSidebarVisibility",
    ],
    "terminal.integrated.allowChords": false, // https://superuser.com/a/1784306/1402
}
```
