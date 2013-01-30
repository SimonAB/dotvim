Installation:

    git clone https://github.com/SimonAB/dotvim.git ~/.vim

Create symlinks:

    ln -s ~/.vim/vimrc ~/.vimrc
    ln -s ~/.vim/gvimrc ~/.gvimrc

Switch to the `~/.vim` directory, and fetch submodules:

    cd ~/.vim
    git submodule init
    git submodule update

Occassionally, the bundles may need updating.  To do this, `cd ~/.vim && ./update`
