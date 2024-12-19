# telescope

[Telescope plugin](https://github.com/nvim-telescope/telescope.nvim).

## searching through files

Config to search through files:

```lua
local builtin = require('telescope.builtin')
vim.keymap.set('n', '<leader>rg', function()
	builtin.grep_string({ search = "" }); -- do live search
end)
```

Then `<c-q>` to send the results to the quickfix list. And `:cnext` and `:cprev` to navigate the quickfix list. `:copen` to open the quickfix list.

