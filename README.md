Installation on a new machine:

    git clone https://github.com/SimonAB/dotvim.git ~/.vim

Create symlinks:

    ln -s ~/.vim/vimrc ~/.vimrc
    ln -s ~/.vim/gvimrc ~/.gvimrc

Switch to the `~/.vim` directory, and fetch submodules:

    cd ~/.vim
    git submodule update --init

To install new plugins:

    git submodule add <github url> bundle/<name>

To commit & upload changes to git:

    git add .
    git commit -m "<description>"
    git push

Occassionally, the bundles may need updating.  To do this:

    git submodule foreach git pull origin master
