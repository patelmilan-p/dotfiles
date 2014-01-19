tricomsol dotfiles
==================

Requirements
------------

set zsh as your login shell.

  chsh -s /bin/zsh

Install [rcm](https://github.com/thoughtbot/rcm):

  Debain-based (including Ubuntu):
    
    wget http://thoughtbot.github.io/rcm/debs/rcm_1.1.0_all.deb
    sudo dpkg -i rcm_1.1.0_all.deb

  OS X:

    brew tap thoughtbot/rcm
    brew install rcm

Install
-------

Clone the repo:

  git clone git://github.com/tricomsol/dotfiles.git

Symlink your dot files:

  rcup -d dotfiles -x README.md

This will create symlinks for config files in your home directory.
The `-x` options, which exclude the `README.md` files, are needed
during installation but can be skipped once the `.rcrc` configuration
file is symlinked in.

You can safely run `rcup` multiple times to update:

  rcup
