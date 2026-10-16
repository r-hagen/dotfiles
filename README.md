# Robert's dotfiles

Personal `dotfiles` managed with [chezmoi](https://www.chezmoi.io/).

## Install

    chezmoi init --apply https://github.com/r-hagen/dotfiles.git

## Requirements

- [chezmoi](https://www.chezmoi.io/) - `brew install chezmoi`
- [git](https://git-scm.com/) - `brew install git`
- [tmux](https://github.com/tmux/tmux) - `brew install tmux`
- [neovim](https://neovim.io/) - `brew install neovim`
- [herdr](https://herdr.dev) - `brew install herdr`
- [jq](https://jqlang.org/) - `brew install jq`
- [bat](https://github.com/sharkdp/bat) - `brew install bat`
- [lazygit](https://github.com/jesseduffield/lazygit) - `brew install lazygit`
- [lazydocker](https://github.com/jesseduffield/lazydocker) - `brew install lazydocker`
- [oh-my-zsh](https://ohmyz.sh/) - `sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"`

## Usage

Change configs through chezmoi, not by editing files in `~` directly.

    chezmoi edit --apply ~/.zshrc   # edit source and apply
    chezmoi add ~/.config/foo/bar   # start managing a file
    chezmoi re-add                  # pull direct edits back into source
    chezmoi status                  # list drift between source and home
    chezmoi diff                    # show what apply would change
    chezmoi update                  # pull from remote and apply

Commit and push from the source directory:

    chezmoi cd
    git add -A && git commit -m "<area>: <summary>" && git push

## Secrets

Secrets are stored in `~/.secrets` (not committed) and sourced by `~/.zshrc`.
