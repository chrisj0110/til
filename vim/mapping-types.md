# Mapping types

Mapping types are listed [here](https://vim.fandom.com/wiki/Mapping_keys_in_Vim_-_Tutorial_(Part_1)#Mode-specific_maps)

```
Commands                        Mode
--------                        ----
nmap, nnoremap, nunmap          Normal mode
imap, inoremap, iunmap          Insert and Replace mode
vmap, vnoremap, vunmap          Visual and Select mode
xmap, xnoremap, xunmap          Visual mode
smap, snoremap, sunmap          Select mode
cmap, cnoremap, cunmap          Command-line mode
omap, onoremap, ounmap          Operator pending mode
```

Note: the noremap commands are preferred to the map commands because it avoids unintended side effects because it won't recursively expand mappings within the command.
