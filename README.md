# Dotfiles for BSPWMxorg-xbacklight
### Packages required:
- bspwm
- sxhkd
- yay
- feh
- polybar
- ranger
- xorg-xsetroot
- xorg-xbacklight
- lxappearance
- w3m
- dmenu
- picom-ibhagwan-git
- st-luke-git
- multilockscreen-git
- thunar
- nerd-fonts-complete
- ttf-font-awesome
- ttf-weather-icons
- flameshot
- dunst 
- neovim
- xdo
- xdotool
- xtitle
- sutils
- fzf
- numlockx

### Install with one command
```
yay -S bspwm-git sxhkd-git feh polybar-git ranger xorg-xsetroot lxappearance w3m dmenu picom-ibhagwan-git st-luke-git multilockscreen-git nerd-fonts-complete ttf-font-awesome flameshot dunst neovim ttf-weather-icons
sudo pacman -Syu xdo xdotool xtitle sutils fzf xorg-xbacklight numlockx thunar
```
### How to copy configs to raw Arch
```
cd
git clone https://github.com/iamm3chanic/dotfiles
cp -r dotfiles/.config/* ~/.config/*
chmod +x ~/.config/bspwm/*
chmod +x ~/.config/sxhkd/*
chmod +x ~/.config/polybar/launch.sh
#copy something... not forget about pictures
```
### Preview

### Shortcuts