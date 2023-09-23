# ale plugin

[Asynchronous Lint Engine](https://github.com/dense-analysis/ale)

`:ALEInfo` to see what is configured for the current file.

Some .vimrc settings I've been playing with so far:

```
let g:ale_completion_enabled = 1  " does this work?
let g:ale_linters_explicit = 1  " Only run linters named in ale_linters settings.
" haven't got jump-to-definition to work yet - see bottom of https://github.com/dense-analysis/ale/issues/2231
" mypy is the slowest, do I need to setup cache?
" let g:ale_linters = {
" \   'python': ['pyright', 'mypy'],
" \}
" let g:ale_fix_on_save = 1
" let g:ale_fixers = {
" \   'python': ['black'],
" \}
let g:ale_python_black_options = '--line-length=160'
nnoremap <F8> :ALENextWrap<CR>
```

