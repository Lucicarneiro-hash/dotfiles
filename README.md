# dotfiles

Personal shell configuration for macOS.

## Files

- `.zshrc` — Zsh configuration: Oh My Zsh, nvm, and PATH setup
- `.zprofile` — Login shell configuration: Homebrew environment

## Setup

Clone the repo and symlink the files to your home directory:

```sh
git clone https://github.com/Lucicarneiro-hash/dotfiles.git ~/dotfiles
ln -sf ~/dotfiles/.zshrc ~/.zshrc
ln -sf ~/dotfiles/.zprofile ~/.zprofile
```

## Tools

- [Oh My Zsh](https://ohmyz.sh)
- [nvm](https://github.com/nvm-sh/nvm)
- [Homebrew](https://brew.sh)
