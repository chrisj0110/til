# commands

## my custom

### panes

- `<prefix> s` - split pane to the bottom
- `<prefix> v` - split pane to the right

## default

### sessions
- `<prefix> L` - switch to previously-used session

### windows

- `<prefix> c` - new window
- `<prefix> <number>` - nth window
- `<prefix> n` - next window, or `p` for previous window
- `<prefix :swap-window -s 2 -t 1` - swap window from 2 to 1
- `<prefix> &` - kill window
- `<prefix> :rename-window my-new-name` - rename window

### panes

- `<prefix> %` - split pane to the right
- `<prefix> "` - split pane to the bottom
- `<prefix> <arrow key>` - navigate to pane in <arrow> direction
- `<prefix> {` - swap pane to the left, or `}` for right
- `<prefix> q` - identify panes, then press number to select
- `<prefix> z` - zoom into pane
- `<prefix> !` - turn pane into a window

### misc

- `<prefix> I` - install new packages from tmux.conf
- `<prefix> [` - start copy mode, `v` to start copy selection, `y` to yank, `c-v` to toggle line vs block
- `<prefix> ]` - paste from copy mode
- `tmux detach` - detach; with `tmux attach` for last session
- `:list-keys` - show all mappings

see also http://tmuxcheatsheet.com/

see also https://github.com/omerxx/dotfiles/blob/master/tmux/tmux.reset.conf

from https://www.youtube.com/watch?v=DzNmUNvnB04 and https://www.youtube.com/watch?v=GH3kpsbbERo
