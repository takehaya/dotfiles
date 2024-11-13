# dotfiles
dotfiles managed by chezmoi.

# usage
```shell
brew install chezmoi

chezmoi init https://github.com/takehaya/dotfiles.git

chezmoi apply

./resymlinked.sh

## Prezto update
zprezto-update

## fail case...
cd .zprezto
git pull
git submodule sync --recursive
git submodule update --init --recursive
```

## update dotfile
```shell
# e.g. update zshrc
vim .zshrc
# or
vim .zprezto/runcoms/zshrc

# update
update_zshrc

# git ops case
cd ~/.local/share/chezmoi
git commit -m "update zsh"
git push
```

# tips
- https://zenn.dev/ryo_kawamata/articles/introduce-chezmoi
