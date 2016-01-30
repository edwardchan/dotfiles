# dotfiles
Dotfiles and symlinks for portability

##Cloning dotfiles to another machine
###Clone this repository
```
git clone git://github.com/edwardchan/dotfiles.git
```
###Make script executable
Once the repository has been cloned into the home directory, change into the `dotfiles` directory and make the `makesymlinks.sh` executable
```
cd ~/dotfiles
chmod +x makesymlinks.sh
./makesymlinks.sh
```
*Warning: If you’re running Debian Linux, this will most likely install `zsh` on your system if it isn’t already installed. This is a feature I added to my script to automate things as much as possible. If for some reason you don’t want `zsh` to be installed on your computer (e.g. you’re on somebody else’s server), remove the `install_zsh` line from `makesymlinks.sh`. This will cause it to set up all of your dotfiles without attempting to install `zsh`.*

That’s it! If the settings don’t take effect right away, just log out and log back in to re-source the dotfiles.
