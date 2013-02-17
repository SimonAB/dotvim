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

To remove a submodule:

1. Delete the relevant section from the .gitmodules file.
2. Delete the relevant section from .git/config.
3. Run git rm --cached path_to_submodule (no trailing slash).
4. Commit and delete the now untracked submodule files.

Occassionally, the bundles may need updating.  To do this:

    git submodule foreach git pull origin master
