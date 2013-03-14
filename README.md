yuanfarn's vimrc
================
Author: Shau-Hung Hsieh <shauhung@gmail.com>

Fork me on GITHUB  https://github.com/yuanfarn/vimrc.git.

MANUALLY INSTALL
----------------

1. Check out from GitHub

        git clone https://github.com/yuanfarn/vimrc.git ~/.vim
        cd ~/.vim
        git submodule init
        git submodule update

2. Install ~/.vimrc

        cd ~ && ln -s ~/.vim/vimrc ~/.vimrc 

3. Install plugin by Vundle, and lunch Vim 

        vim +BundleInstall 

INSTALL & UPGRADE PLUGIN BUNDLES
--------------------------------

To install a new plugin by Vundle, just add a new line to .vimrc

    Bundle [USER-NAME/PLUGIN-NAME]

For example, if you want to install `vim-markdown` (https://github.com/plasticboy/vim-markdown), then add this line to .vimrc

    Bundle 'plasticboy/vim-markdown'

Here, `plasticboy` is username. If the username is `vim-scripts` (http://vim-scripts.org/), you can ignore it.

Also, you can install a new plugin as a git submodule, type the following commands.

    cd ~/.vim
    git submodule add [GIT-REPOSITORY-URL] bundle/[PLUGIN-NAME]

In this project, `Pathogen` and `Vundle` are installed as git submodule. But, `SrcExpl`, `Trinity`, `taglist.vim`, and `Nerd Tree` are installed by using Vundle.

PLUGINS
-------

* [Pathogen](http://www.vim.org/scripts/script.php?script_id=2332): Pathogen let us install a plugin as a bundle in ~/.vim/bundle seprately.

* [Vundle](https://github.com/gmarik/vundle): To manage your scripts right in .vimrc

  Useful commands:   
    `:BundleInstall` - Installing requires Git and triggers Git clone for each configured repo to ~/.vim/bundle/   
    `:BundleInstall!` - Update your scripts   
    `vim +BundleInstall` - Installing requires Git and lunch Vim.   

* [SrcExpl](https://github.com/vim-scripts/SrcExpl.git): Source Explorer, which can work with 'Taglist' and 'NERD tree'.

* [Trinity](https://github.com/vim-scripts/Trinity.git): To manage Source Explorer, Taglist and NERD Tree.

* [taglist.vim](https://github.com/vim-scripts/taglist.vim.git): To provide an overview of the structure of source code files.

* [Nerd Tree](https://github.com/vim-scripts/The-NERD-tree.git): A tree explorer plugin for navigating the filesystem.

  Useful commands:   
    `:Bookmark [name]` - bookmark any directory as name   
    `:NERDTree [name]` - open the bookmark [name] in Nerd Tree   

History
-------

Mar 14, 2013: Initial this project. The major reference is vgod's vimrc (https://github.com/vgod/vimrc).

License
-------

This vimrc project is released under [Creative Commons Attribution-ShareAlike 3.0 Unported License](http://creativecommons.org/licenses/by-sa/3.0/deed.en_US).

