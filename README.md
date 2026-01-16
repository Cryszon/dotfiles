# Cryszon's dotfiles

This repository contains my personal dotfiles that I manage with
[chezmoi](https://github.com/twpayne/chezmoi) along with some app and
customization notes.

If you find something useful, feel free to copy and modify.

For more configuration files, check out [Reun Media Project
Templates](https://github.com/ReunMedia/project-templates) and [Reun Media PHP
app template](https://github.com/ReunMedia/php-app-template).

## Quick Start

Install [Essential Tools](#essential-tools):

```
curl -sS https://starship.rs/install.sh | sh
brew install fzf
```

Install [chezmoi](https://github.com/twpayne/chezmoi):

```
brew install chezmoi
```

Initialize and apply dotfiles:

```
chezmoi init --apply Cryszon
```

## Essential Tools

These are the tools I install on almost every machine I manage. I've written
down quick install commands for myself below. For more information, check out
the respective tools' websites.

### [Starship](https://starship.rs/)

```sh
curl -sS https://starship.rs/install.sh | sh
```

Starship is automatically enabled if installed. Run `source ~/.bashrc` to enable
it in the current shell.

### [fzf](https://junegunn.github.io/fzf/)

With [Homebrew](https://brew.sh/) (recommended):

```sh
brew install fzf
```

Without Homebrew:

1. Download latest binary from
   [releases](https://github.com/junegunn/fzf/releases)

   ```sh
   wget https://github.com/junegunn/fzf/releases/download/???.tar.gz`
   ```

2. Install to `$PATH`

   ```sh
   tar -xvzf fzf-???.tar.gz -C /usr/local/bin
   ```

fzf is automatically enabled if installed. Run `source ~/.bashrc` to enable it
in the current shell.

## Almost Essential Tools

### [tmux](https://github.com/tmux/tmux)

```
sudo apt install tmux
```

### [btop](https://github.com/aristocratos/btop)

```
sudo apt install btop
```

## Theme

[Catppuccin Mocha](https://catppuccin.com/) is my preferred theme. Here are
links to various ports I use it in:

- [Gnome Terminal](https://github.com/catppuccin/gnome-terminal)
- [Gnome Text Editor](https://github.com/catppuccin/gnome-text-editor)
- [btop](https://github.com/catppuccin/btop)
- [VS Code](https://github.com/catppuccin/vscode) (automatically synced)

## Additional notes

### Neovim as Vim alternative

```sh
update-alternatives --config vim
```
