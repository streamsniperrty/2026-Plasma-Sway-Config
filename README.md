# 2026 Plasma and Hyprland Config Guide

Welcome! This guide will go over how I customized KDE Plasma 6 as well as the Hyprland window manager.

![Plasma Home](/imgs/plasma_home.png)

Plasma Tricks
- Global theme: Layan
  - Window Decorations: Layan

- Icon Pack: Tela
- Dock Digital Time: Command Output by Zren

Fonts Used:
- Arimo (sans-serif)
- Tinos (serif)
- Cousine (monospace)

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
The only thing that I changed is the font. To change the font, go to `$HOME/.config/rofi/launchers/type-2/shared/fonts.rasi`. Use Arimo.
