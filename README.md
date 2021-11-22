# setup

> Steps to set up my Linux environment

## Install Packages

```bash
sudo apt install git fish neovim
```

## Neovim

- Install vim-plug

```
sh -c 'curl -fLo "${XDG_DATA_HOME:-$HOME/.local/share}"/nvim/site/autoload/plug.vim --create-dirs \
       https://raw.githubusercontent.com/junegunn/vim-plug/master/plug.vim'
```

- Open `init.vim`

```
nvim ~/.config/nvim/init.vim
```

- Copy `init.vim` from [dotfiles](https://github.com/mathletedev/dotfiles) into file

- Save and source

```
:w
:source %
```

- Install plugins

```
:PlugInstall
```

## Fish

- Install oh-my-fish

```
curl https://raw.githubusercontent.com/oh-my-fish/oh-my-fish/master/bin/install | fish
```

- Install bobthefish

```
omf install bobthefish
```

- Open `config.fish`

```
nvim ~/.config/fish/config.fish
```

- Copy `config.fish` from [dotfiles](https://github.com/mathletedev/dotfiles) into file

## Node

- Install Fisher

```
curl -sL https://git.io/fisher | source && fisher install jorgebucaran/fisher
```

- Install nvm

```
fisher install jorgebucaran/nvm.fish
```

- Install latest version of node

```
nvm install latest
```

- To use another version of node

```
set --universal nvm_default_version vx.x.x
```
