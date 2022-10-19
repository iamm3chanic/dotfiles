# Dotfiles for BSPWM
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
- htop
- sublime-text-3
- evince
- thunar 
- firefox
- parole
- cava
- conky

### Install with one command
```
yay -S polybar-git ranger-git picom-ibhagwan-git st-luke-git \
multilockscreen-git nerd-fonts-complete ttf-weather-icons 
xtitle sutils sublime-text-3 cava

sudo pacman -Syu bspwm sxhkd xdo xdotool fzf xorg-xbacklight \
numlockx thunar dunst neovim flameshot ttf-font-awesome feh \
xorg-xsetroot lxappearance w3m dmenu htop evince thunar \
firefox parole conky
```
### How to copy configs to raw Arch
```
cd
git clone https://github.com/iamm3chanic/dotfiles
cp -r dotfiles/.config/* ~/.config/
cp dotfiles/.conkyrc ~/.conkyrc
chmod +x ~/.config/bspwm/*
chmod +x ~/.config/sxhkd/*
chmod +x ~/.config/polybar/launch.sh
chmod +x ~/.conkyrc
mkdir -p Pictures
mkdir -p Pictures/screenshots
cp dotfiles/PREVIEW/arch-pic-wall.jpg Pictures/
cp dotfiles/.fehbg ~/
cp dotfiles/.Xresources ~/
cp dotfiles/.xinitrc ~/
chmod +x .xinitrc .Xresources .fehbg
```
### Preview
![help menu](https://raw.githubusercontent.com/iamm3chanic/dotfiles/main/PREVIEW/help_menu.png) 
![ranger evince](https://raw.githubusercontent.com/iamm3chanic/dotfiles/main/PREVIEW/ranger_evince.png)
![neofetch float](https://raw.githubusercontent.com/iamm3chanic/dotfiles/main/PREVIEW/neo.png)
![mc htop](https://raw.githubusercontent.com/iamm3chanic/dotfiles/main/PREVIEW/mc_htop.png)  
![cava](https://raw.githubusercontent.com/iamm3chanic/dotfiles/main/PREVIEW/cava.png)
![neofetch subl](https://raw.githubusercontent.com/iamm3chanic/dotfiles/main/PREVIEW/neofetch.png)

### Shortcuts
COMMAND | MEANING
--- | --- 
super + Return  |        # terminal emulator
super + F1  |    # show help on key bindings
super + d  |     # program launcher
alt + w  |       # firefox
alt + s  |       # sublime text3
alt + f  |       # thunar
super + Print  |         # flameshot gui
super + l  |     # Lockscreen
ctrl + alt + Delete  |   # To lxdm
super + alt + s  |       # Shutdown
super + Escape  |        # make sxhkd reload its configuration files:
alt + 0  |       # volume +
alt + 9  |       # volume -
ctrl + 0  |      # brightness +
ctrl + 9  |      # brightness -
super + shift + r  |     # quit/restart bspwm
super + shift + q  |     # close and kill
super + m  |     # alternate between the tiled and monocle layout
super + y  |     # send the newest marked node to the newest preselected node
super + g  |     # swap the current node and the biggest node
super + shift + space  |         # Toggle floating
super + e  |     # Toggle horizontal/vertical
super + f  |     # Fullscreen
super + shift + t  |     # set the window state
super + ctrl + {m,x,y,z}  |      # set the node flags
super + {_,shift + }{h,j,k,l}  |         # focus the node in the given direction
super + {_,shift + }c  |         # focus the next/previous node in the current desktop
super + bracket{left,right}  |   # focus the next/previous desktop in the current monitor
super + {grave,Tab}  |   # focus the last node/desktop
super + {o,i}  |         # focus the older or newer node in the focus history
super + shift + {1-9,0}  |       #send to the given desktop
super + {1-9,0}  |       # focus to given desktop
super + {v,n}  |         # Set preselection
super + ctrl + {1-9}  |  # preselect the ratio
super + ctrl + space  |  # cancel the preselection for the focused node
super + ctrl + shift + space  |  # cancel the preselection for the focused desktop
super + ctrl + p   |     # Move node to preselect
super + alt + {h,j,k,l}  |       # expand a window by moving one of its side outward
super + alt + shift + {h,j,k,l}  |       # contract a window by moving one of its side inward
super + alt + shift + {Left,Down,Up,Right}  |    # contract a window by moving one of its side inward
super + ctrl + {Left,Down,Up,Right}  |   # move a floating window
super + F11  |   # hide node
super + shift + F11  |   # unhide node

### Possible issues
#### 1. Polybar
If you can't see battery, wi-fi or volume icon on tray, edit ~/.config/polybar/config.  
Follow [Polybar Wiki](https://github.com/polybar/polybar/wiki/Configuration)

#### 2. Bspwm
Check if all configuration files are executable.

#### 3. Sxhkd
Make your own shortcuts in `~/.config/sxhkd/sxhkdrc` and don't forget to reload them! 
```
pkill -USR1 -x sxhkd
```
#### 4. Write to issues and explain what else is wrong :)
