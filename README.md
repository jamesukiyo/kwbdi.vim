# kwbdi.vim improved improved

## Notes from the original repo
This is a mirror of http://www.vim.org/scripts/script.php?script_id=2103

This is an improved improved version of kwbd.vim. It allows you to delete a buffer without closing the window. It meets the following criteria:

    * The window layout must be kept in all circumstances.
    * If there is an alternate buffer must be showing that.
    * If there is not alternate buffer then must be showing the preious buffer.
    * If there is no alternate nor previous buffer (it is the only buffer) must show an empty buffer. 

If there are two windows with the same buffer open, both windows will remain open, and the buffer will be deleted

Thanks to the authors of kwbd.vim and minibufexpl.vim!

## Notes from me
I've removed the default force deletion of buffers `bd!` from the original plugin.

Also removed the default mapping.

Thanks to the authors of kwbdi.vim, kwbd.vim and minibufexpl.vim!

## Install
vim-plug:
```
Plug 'jamesukiyo/kwbdi.vim'
```

## Usage
There are no default mappings so add your own in your .vimrc like so:
```
map <Leader>qb <Plug>Kwbd
```
