" Basic Configurations on Vim, basic configuratons.
" Date: July 12, 2024
" Reference: https://github.com/vim/vim/blob/master/runtime/defaults.vim

set nocompatible
set backspace=indent,eol,start
set ruler 

"-------- General Settings --------
"-> history limit.
set history=500
"-> choose theme.
colorscheme = homebrew
"-> 
set nomodeline
"-> enable syntax highlighting
syn on


"-------- Text and Indent Settings -------- 
"-> show number line 
set number
"-> which to cursorline to show current line.
set nocursorline
"-> enable mouse support.
set mouse=a
"-> show matching parentheses.
set showmatch
"-- auto indentations --
"-> general indent setting
set autoindent
"-> number of characters to indent by.
set shiftwidth=4
"-> number of characters for tab key.
set tabstop=4
"-> set tab character to expand as spaces.
set expandtab


"-------- Custom Settings --------
"-> Map F2 key to save file in Normal mode
nnoremap <F2> :w<CR>
"-> Map F2 key to save file in Insert mode
inoremap <F2> <C-o>:w<CR>
"-> Map F3 key to save and quit file in Normal mode
nnoremap <F3> :wq<CR>
"-> Map F4 key to clear file contents in Normal mode
nnoremap <F4> ggdG
"-> Map F5 key to copy entire contents of file to clipboard
nnoremap <F5> :%y+<CR>


"-> Ctrl+f to move to end of word
inoremap <C-f> <Esc>ea
"-> Ctrl+b to move to beginning of word
inoremap <C-b> <C-Left>
"->  Ctrl+a to move to end of line
inoremap <C-a> <End>
"-> Can't use Ctrl+i remapping as it affects Tab as well
inoremap <C-s> <Home>



" Other useful vimrcs and links
" https://github.com/vim/vim/blob/master/runtime/defaults.vim
" https://github.com/romainl/idiomatic-vimrc/blob/master/idiomatic-vimrc.vim
" https://vi.stackexchange.com/questions/2003/how-do-i-debug-my-vimrc-file
