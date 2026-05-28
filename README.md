# dotfiles

> [https://github.com/Lucicarneiro-hash/dotfiles](https://github.com/Lucicarneiro-hash/dotfiles)

Personal shell configuration for macOS and Windows (via WSL).

## Files

- `.zshrc` — Zsh configuration: Oh My Zsh, nvm, and PATH setup
- `.zprofile` — Login shell configuration: Homebrew environment (macOS only)

## Setup

### macOS

Clone the repo and symlink the files to your home directory:

```sh
git clone https://github.com/Lucicarneiro-hash/dotfiles.git ~/dotfiles
ln -sf ~/dotfiles/.zshrc ~/.zshrc
ln -sf ~/dotfiles/.zprofile ~/.zprofile
```

### Windows (WSL)

These dotfiles work on Windows via [WSL](https://learn.microsoft.com/en-us/windows/wsl/install) with a Zsh shell.

1. Install WSL and a Linux distro (Ubuntu recommended):
   ```powershell
   wsl --install
   ```

2. Inside WSL, install Zsh and Oh My Zsh:
   ```sh
   sudo apt update && sudo apt install -y zsh
   sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
   ```

3. Clone the repo and symlink `.zshrc` (`.zprofile` is macOS/Homebrew-specific):
   ```sh
   git clone https://github.com/Lucicarneiro-hash/dotfiles.git ~/dotfiles
   ln -sf ~/dotfiles/.zshrc ~/.zshrc
   ```

4. Install nvm:
   ```sh
   curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.40.0/install.sh | bash
   ```

## Tools

- [Oh My Zsh](https://ohmyz.sh)
- [nvm](https://github.com/nvm-sh/nvm)
- [Homebrew](https://brew.sh) (macOS)
- [WSL](https://learn.microsoft.com/en-us/windows/wsl/install) (Windows)
