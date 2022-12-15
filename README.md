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

- how do i manange my dotfiles
  - here is an article in archwiki and hackernews
    > > https://news.ycombinator.com/item?id=11071754
    > > https://wiki.archlinux.org/title/Dotfiles
- but simpler explanation

```
    $ git init --bare ~/.dotfiles

    $ alias config='/usr/bin/git --git-dir=$HOME/.dotfiles/ --work-tree=$HOME'

    $ config config status.showUntrackedFiles no

    $ config status
    $ config add .vimrc
    $ config commit -m "Add vimrc"
    $ config add .config/redshift.conf
    $ config commit -m "Add redshift config"
    $ config push
```
