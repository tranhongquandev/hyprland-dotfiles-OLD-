

### PREVIEW

<div align="justify">
    <div align="center">
      <img src="https://github.com/theshy-arch/hyprland-dotfiles/assets/95228594/99761551-9592-405c-bc72-e41cb56c360a" alt="preview.png">
</div> 

## Programs and other resources used

- WM: [hyprland](https://hyprland.org/)

- Wallpaper: [swaybg](https://github.com/swaywm/swaybg)

- Terminal: [Kitty](https://sw.kovidgoyal.net/kitty/)

- Shell: [zsh](https://wiki.archlinux.org/index.php/zsh)

- Fetch tool: [Neofetch](#)

- Zsh prompt: [Starship](https://starship.rs/)

- Bar: [Waybar](https://github.com/Alexays/Waybar)

- Launcher: [Rofi](https://github.com/davatorium/rofi)

- File manager: [Thunar](#)

- Network: [Network-manager-applet](#)

-  Fonts : [JetBrains Mono](#) , [ttf-font-awesome](#), [Fira Code](#)

- Notifications: [Mako](https://github.com/emersion/mako)

- Audio: [Pipewire](https://pipewire.org/) + [wireplumber](https://pipewire.pages.freedesktop.org/wireplumber/)
    , [pavacontrol](#), [pulseaudio](#),[alsa-utils](#)

### Other dependances

- [swayidle](https://github.com/swaywm/swayidle): lock the session before hibernating/suspending

- [waybar-hyprland](https://aur.archlinux.org/packages/waybar-hyprland): waybar but the workspaces widget works with hyprland

- [wlogout](https://github.com/ArtsyMacaw/wlogout): logout window for wayland

## Installation
- First, you need install some things important to have running for a smooth Wayland/Hyprland in <a href="https://wiki.hyprland.org/Useful-Utilities/Must-have/">here</a>

- Clone [gruvbox branch](https://github.com/theshy-arch/hyprland-dotfiles/tree/gruvbox) : 
```shell
git clone -b gruvbox https://github.com/theshy-arch/hyprland-dotfiles
```

-  Install these and then copy my config files into your ~/.config folder

```shell
yay -S kitty hyprland-git waybar-hyprland-git xdg-desktop-portal-hyprland pipewire wireplumber grim slurp pulseaudio pavucontrol brightnessctl alsa-utils xf86-video-intel thunar swaybg ttf-font-awesome rofi neofetch htop cava wlogout mako polkit-gnome qt6-wayland
```

## Install Fonts

- Install  font awesome : ``` yay -S  ttf-font-awesome ```

- Clone <a href="https://github.com/theshy-arch/fotns">this repo</a> and copy all file .tff to ``` ~/.local/share/fonts``` 
then run : ``` fc-cache -f -v ```

## SHELL Setups
 
- First of all install fish based on your Linux distributions:

```shell

pacman -S fish

```
- Then  install  [StarShip Promt](https://starship.rs/) :
```shell
    
    curl -sS https://starship.rs/install.sh | sh
    
```
- Also, if you want the terminal icon install exa using <a href="https://the.exa.website/install">this</a> guide
- Finally,  add this command to ``` ~/.config/fish/config.fish ``` and copy file ```starship.toml``` to ```~/.config/```
    
    ```shell
    
    starship init fish | source
    set fish_greeting
    neofetch
    
    ```

## Other

- if you want to type Vietnamese keyboard,  install this :

```shell

sudo pacman -S fcitx5 fcitx5-qt fcitx5-gtk fcitx5-unikey  kcm-fcitx5

```
- Add this command to ``` /etc/environment/ ```. Then, add command ``` exec-once=fcitx5 -D ``` to ```hyprland.conf ```

```shell
GTK_IM_MODULE=fcitx
QT_IM_MODULE=fcitx
XMODIFIERS=@im=fcitx

```
Finally, add input keyboard layout ```Unikey``` in fcitx5 configuration GUI

## Special thanks to 

-  https://github.com/0bCdian/Hyprland_dotfiles for the base config
