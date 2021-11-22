# setup

> Steps to set up my Linux environment

## Install Packages

```bash
sudo apt install git fish neovim
```

## Neovim

- Install vim-plug

```bash
sh -c 'curl -fLo "${XDG_DATA_HOME:-$HOME/.local/share}"/nvim/site/autoload/plug.vim --create-dirs \
       https://raw.githubusercontent.com/junegunn/vim-plug/master/plug.vim'
```

- Open `init.vim`

```bash
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

```bash
curl https://raw.githubusercontent.com/oh-my-fish/oh-my-fish/master/bin/install | fish
```

- Install bobthefish

```bash
omf install bobthefish
```

- Open `config.fish`

```bash
nvim ~/.config/fish/config.fish
```

- Copy `config.fish` from [dotfiles](https://github.com/mathletedev/dotfiles) into file

## Node

- Install Fisher

```bash
curl -sL https://git.io/fisher | source && fisher install jorgebucaran/fisher
```

- Install nvm

```bash
fisher install jorgebucaran/nvm.fish
```

- Install latest version of node

```bash
nvm install latest
```

- To use another version of node

```bash
set --universal nvm_default_version vx.x.x
```
