# .dotfiles

Dotfiles for my Arch Linux

## how to backup dotfiles

> git init $HOME/.dotfiles

> alias dots='git --git-dir=$HOME/.dotfiles/.git --work-tree=$HOME'

> echo "alias dots='git --git-dir=$HOME/.dotfiles/.git --work-tree=$HOME'" >> $HOME/.zshrc

> source $HOME/.zshrc

> dots config --local status.showUntrackedFiles no

> dots add .vimrc .zshrc

> dots commit -m "Initial Commit"

> dots push

> ln -f
