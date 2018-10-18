# hyperwsl
Simple configs and notes for using Windows Subsystem for Linux, bash and hyper terminal for grooviness - this is the bare skeleton bones of what I did: I will flash out and improve ASAP

Install wsl from add windows features - search add features and you will fine the 'Turn windows features on or off'

Install ubuntu from the windows store

Install hyper terminal https://hyper.is/

Replace existing contents of .hyper file with my .hyperfile - to do so with hyper open type cntrl + , then copy and paste my contents into the prefs file - then save from the file menu.

Then in wsl:

sudo apt-get install screenfetch

 sudo apt-get install zsh
 
 vim ~/.zshrc
 
 add this
 
 # Set name of the theme to load. Optionally, if you set this to "random"
# # it'll load a random theme each time that oh-my-zsh is loaded.
# # See https://github.com/robbyrussell/oh-my-zsh/wiki/Themes
ZSH_THEME="agnoster"

vim ~/.bashrc

add this to set it to use zsh

# ~/.bashrc: executed by bash(1) for non-login shells.
# see /usr/share/doc/bash/examples/startup-files (in the package bash-doc)
# for examples
screenfetch
bash -c zsh
# ~/.bashrc: executed by bash(1) for non-login shells.
# see /usr/share/doc/bash/examples/startup-files (in the package bash-doc)
# for examples
# If not running interactively, don't do anything
case $- in

# If not running interactively, don't do anything
case $- in
    *i*) ;;
      *) return;;
esac

## install oh my zsh
sh -c "$(curl -fsSL https://raw.githubusercontent.com/robbyrussell/oh-my-zsh/master/tools/install.sh)"


Enjoy
