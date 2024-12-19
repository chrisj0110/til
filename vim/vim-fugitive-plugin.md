# vim-fugitive plugin

https://github.com/tpope/vim-fugitive

- `:G` - git status
    - `s` - stage
    - `u` - unstage
    - `=` - inline diff
        - `=s` - to stage file when looking at a hunk
    - `dv` - diff vertical
    - `X` - restore
    - `cc` - commit
    - `)` - next hunk
    - `(` - previous hunk
    - `co ` - populates with ":Git checkout "

- `:Gvdiffsplit` - git diff
    - `:Gvdiffsplit branchname` - diff vs branchname

- `:G difftool -y` - diffs for all files in tabs
    - `:tabo` to close all but the current tab

- `:G log` - git log
    - `o` - see the diff of the commit

- `:G blame` - git blame
    - `<CR>` on the commit to see the change. `<ctrl-o>` to go back.

- `:G push` - git push

- `:Gedit branchname:file.txt` - open file.txt from branchname

