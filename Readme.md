# Dotfiles

This repository contains *nix user config files that I'd like to carry over in between systems.

My setup is pretty minimal on top of Ubuntu/Gnome. I also try not to carry over too much when setting up a new system. I find that it's a good time to clear house on the junk I'm not actually using.

## Setup

Create symbolic links between the files in this repository to the home directory.

```bash
ln -s "$(pwd)/.bash_aliases" ~/.bash_aliases
ln -s "$(pwd)/.inputrc" ~/.inputrc
ln -s "$(pwd)/.gitconfig" ~/.gitconfig

# Ergodox keyboard layouts
mkdir -p ~/Tools/ergodox
ln -s "$(pwd)/ergodox_layouts" ~/Tools/ergodox/layouts
```

## Install

- vscode
- git via `ppa:git-core/ppa`

## Essential Non-Package-Manager Install

- The Ergodox firmware flashing tool a.k.a. "wally". Put it in `~/Tools/ergodox`
- [icc-brightness](https://github.com/udifuchs/icc-brightness) if brightness controls aren't working
