## PREVIEW

<div align="justify">
    <div align="center">
            <img src="https://github.com/theshy-arch/hyprland-dotfiles/assets/95228594/825ec5ec-ce50-450a-888e-a0c98316b46d" alt="catppuccin">
    </div>
</div>

## Installation

- Install requirement packages :  
```shell
yay -S hyprland-git waybar-hyprland wofi dunst kitty swaybg swayidle  brightnessctl pavucontrol alsa-utls  thunar grim slurp network-manager-applet lf neovim cava btop neofetch pulseaudio x86-video-intel xdg-desktop-portal-hyprland polkit-gnome qt6-wayland
```

- Clone this [branch](https://github.com/theshy-arch/hyprland-dotfiles/tree/catppuccin) :
```shell
    git clone -b catppuccin https://github.com/theshy-arch/hyprland-dotfiles
```
- Copy all file to ``` ~/.config/```


## Install Fonts

- Awesome font : ``` yay -S ttf-font-awesome ```
- Clone this [branch](https://github.com/theshy-arch/hyprland-dotfiles/tree/fonts) :
```shell
git clone -b fonts https://github.com/theshy-arch/hyprland-dotfiles
````
- Copy all file ```.ttf``` to ```~/.local/share/fonts``` then run command ```fc-cache -f -v```

## SHELL Setups

- Install [Fish shell](https://fishshell.com/) :
```shell
 pacman -S fish 
 ```
 - Change default shell to ```fish```:
 ```shell
    chsh -s /usr/bin/fish
 ```
- Install [Oh-my-fish](https://github.com/oh-my-fish/oh-my-fish) and [themes](https://github.com/catppuccin/fish)

- Install [StarShip Prompt](https://starship.rs/guide/#%F0%9F%9A%80-installation)
 ```shell
 pacman -S starship
 ```
- Add this command to ```~/.config/fish/config.fish```
```shell

starship init fish | source
set fish_greeting
neofetch

```
- Copy file ```starship.toml ``` to ```~/.config/```

## Special thanks to
https://github.com/1amSimp1e/dots for base configs
