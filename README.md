install Pathogen to ~/.vim/bundle/ first:

```
git submodule add git://github.com/tpope/vim-pathogen.git ./vim-pathogen
```
add it to ~/.vimrc:
```
runtime bundle/vim-pathogen/autoload/pathogen.vim
call pathogen#infect()
Helptags
```
and install NERDTree if you want:
```
git submodule add git://github.com/scrooloose/nerdtree.git ./nerdtree
```
add it to ~/.vimrc:
```
nnoremap :NERDTree
```
add YouCompleteMe

must to install cmake
```
/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"

brew install cmake

git clone https://github.com/ycm-core/YouCompleteMe.git

git submodule update --init --recursive

./install.py --clang-completer
```
add rainbow_parentheses
```
git clone https://github.com/kien/rainbow_parentheses.vim.git
```
add to ~/.vimrc
```
let g:rbpt_colorpairs = [
                        \ ['brown',       'RoyalBlue3'],
                        \ ['Darkblue',    'SeaGreen3'],
                        \ ['darkgray',    'DarkOrchid3'],
                        \ ['darkgreen',   'firebrick3'],
                        \ ['darkcyan',    'RoyalBlue3'],
                        \ ['darkred',     'SeaGreen3'],
                        \ ['darkmagenta', 'DarkOrchid3'],
                        \ ['brown',       'firebrick3'],
                        \ ['gray',        'RoyalBlue3'],
                        \ ['darkmagenta', 'DarkOrchid3'],
                        \ ['Darkblue',    'firebrick3'],
                        \ ['darkgreen',   'RoyalBlue3'],
                        \ ['darkcyan',    'SeaGreen3'],
                        \ ['darkred',     'DarkOrchid3'],
                        \ ['red',         'firebrick3'],
                        \ ]
let g:rbpt_max = 16
let g:rbpt_loadcmd_toggle = 0
au VimEnter * RainbowParenthesesToggle
au Syntax * RainbowParenthesesLoadRound
au Syntax * RainbowParenthesesLoadSquare
au Syntax * RainbowParenthesesLoadBraces
```
add ale
```
git clone https://github.com/dense-analysis/ale.git
```
