This plugin is forked from [psf/black](https://github.com/psf/black) and do some modifications.

* Install
```shell
pip install black
```

```viml
Plug 'wzzju/black.vim'
```

* Setting
```viml
" use black to format python files
let g:black_skip_string_normalization = 1
let g:black_linelength = 100
autocmd FileType python nnoremap <buffer><Leader>p :<C-u>Black<CR>
autocmd FileType python vnoremap <buffer><Leader>p :BlackVisual<CR>
autocmd BufWritePre *.py silent execute ':Black'
```
