# Robert's dotfiles

Personal `dotfiles` managed with [chezmoi](https://www.chezmoi.io/).

## Install

    chezmoi init --apply https://github.com/r-hagen/dotfiles.git

## Requirements

- [chezmoi](https://www.chezmoi.io/) - `brew install chezmoi`
- [git](https://git-scm.com/) - `brew install git`
- [tmux](https://git-scm.com/) - `brew install tmux`
- [neovim](https://neovim.io/) - `brew install neovim`
- [oh-my-zsh](https://ohmyz.sh/) - `sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"`

## Secrets

Secrets are stored in `~/.secrets` (not committed) and sourced by `~/.zshrc`.
