 # ubuntu-configuration

# fedora-configuration
## script to setup terminal in fedora

### either configure zsh and oh-my-zsh
```
# if wanting to install zsh, otherwise run with just sh
sudo dnf install zsh
chsh -s $(which zsh)
sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
# change theme to pygmalion
```

### Or keep bash and install oh-my-posh
```
#installing oh-my-posh
sudo dnf install git vim neovim curl tmux
curl -s https://ohmyposh.dev/install.sh | sh -s -- -t /home/arcanegrape/.themes
# add to ~/.bashrc
eval "$(oh-my-posh init bash)"

#install any nerdfont for proper rendering of symbols in oh-my-posh
```

### setting my configuration for vim and tmux
```
curl -o .vimrc https://raw.githubusercontent.com/arcanegrape/ubuntu-configuration/main/.vimrc
curl -o .tmux.conf https://raw.githubusercontent.com/arcanegrape/ubuntu-configuration/main/.tmux.conf

git clone https://github.com/tmux-plugins/tpm ~/.tmux/plugins/tpm
git clone https://github.com/christoomey/vim-tmux-navigator.git ~/.vim/pack/plugins/start/vim-tmux-navigator
```
