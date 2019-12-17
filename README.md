install Pathogen to ~/.vim/bundle/ first:

git submodule add git://github.com/tpope/vim-pathogen.git ./vim-pathogen

add it to ~/.vimrc:

runtime bundle/vim-pathogen/autoload/pathogen.vim

call pathogen#infect()

Helptags

and install NERDTree if you want:

git submodule add git://github.com/scrooloose/nerdtree.git ./nerdtree

add it to ~/.vimrc:

nnoremap :NERDTree
