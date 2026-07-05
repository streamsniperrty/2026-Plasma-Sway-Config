# 2026 Plasma and Sway Config Guide

Welcome! This guide will go over how I customized KDE Plasma 6 as well as the Sway window manager.

![Plasma Home](/imgs/plasma_home.png)

## Plasma Configuration
- Global theme: Layan
  - Window Decorations: Layan

- Icon Pack: Tela
- Dock Digital Time: Command Output by Zren

Fonts Used:
- Arimo (sans-serif)
- Tinos (serif)
- Cousine (monospace)

## Sway Configuration

Here are the critical packages required for sway.
- sway
- swaybg
- swaylock
- waybar

Copy the config files for sway and waybar.

Install the following packages for sway.
- fish
- nvim
- rofi
- kitty
- swaync (called sway-notification-center on Ubuntu repo)
- Hermit Monospaced Font

Copy the config files for fish, nvim, rofi, and kitty in the appropriate locations.

### Installating Rofi
This is documented on the official repo: https://github.com/adi1090x/rofi

First, Make sure you have the same (stable) version of rofi installed.
- On Arch / Arch-based : sudo pacman -S rofi
- On Debian / Ubuntu : sudo apt-get install rofi
- On Fedora : sudo dnf install rofi

Then, Clone this repository -

` $ git clone --depth=1 https://github.com/adi1090x/rofi.git `

Change to cloned directory and make setup.sh executable -

```
$ cd rofi
$ chmod +x setup.sh
```

Copy config.rasi from this repo to `~/.config/rofi/` on your system.

The only things that I changed are the font and color scheme. To change the font, go to `$HOME/.config/rofi/launchers/type-2/shared/fonts.rasi`. Use Arimo. To change the color scheme, go to `$HOME/.config/rofi/launchers/type-2/shared/colors.rasi` and select `dracula`.

### Installing NeoVim
First, install neovim normally through your package manager. Once completed, install `vim-plug` from https://github.com/junegunn/vim-plug. Then, copy the four files into your own file system, and sync all the plugins by running: `:PlugInstall`.

To use the tree file browser, run `:NvimTreeOpen`.

** NOTE: You will need to update the notification daemon on KDE Plasma once you install `sway-notification-client`. Follow instructions on how to revert to the KDE Plasma notifications.
