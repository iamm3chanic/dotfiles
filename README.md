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
yay -S bspwm-git sxhkd-git polybar-git ranger-git picom-ibhagwan-git st-luke-git multilockscreen-git nerd-fonts-complete ttf-weather-icons xtitle sutils 
sudo pacman -Syu xdo xdotool fzf xorg-xbacklight numlockx thunar dunst neovim flameshot ttf-font-awesome feh xorg-xsetroot lxappearance w3m dmenu 
```
### How to copy configs to raw Arch
```
cd
git clone https://github.com/iamm3chanic/dotfiles
cp -r dotfiles/.config/* ~/.config/*
chmod +x ~/.config/bspwm/*
chmod +x ~/.config/sxhkd/*
chmod +x ~/.config/polybar/launch.sh
mkdir -p Pictures
mkdir -p Pictures/screenshot
cp dotfiles/arch-pic-wall.jpg Pictures/
cp dotfiles/.fehbg ~/
#copy something... not forget about pictures
```
### Preview

### Shortcuts