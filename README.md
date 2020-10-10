## :art: Screenshot

![SS](/Other/screen1.png)

## :snowflake: My Setup :snowflake:

- **WM :** i3wm
- **Terminal :** urxvt
- **Shell :** zsh
- **Panel :** tint2
- **Notification :** dunst
- **App launcher :** rofi
- **File manager :** thunar

## :wrench: Installation

### :computer: **Arch Linux (Dependencies)**

> :exclamation: For AUR helper, im using **yay**

> :page_with_curl: **i3 Windows Manager**

```bash
sudo pacman -S i3-gaps
```

> :sound: **Audio**

```bash
sudo pacman -S alsa-utils pulseaudio
```

> :high_brightness: **Brightness**

```bash
yay -S brightnessctl
```

> :chart_with_upwards_trend: **Network Monitor & RAM Usage**

```bash
yay -S psuinfo
```

> :signal_strength: **Wireless Tools**

```bash
sudo pacman -S wireless_tools
```

> :hammer: **Other utility (panel, notification, terminal, file manager, etc)**

```bash
yay -S dunst tint2 gsimplecal rofi feh lxappearance qt5ct qt5-styleplugins lxsession xautolock rxvt-unicode-patched xclip scrot thunar thunar-archive-plugin thunar-media-tags-plugin thunar-volman tumbler w3m geany nano vim viewnior pavucontrol parcellite neofetch htop picom gtk2-perl zsh zsh-completions imagemagick playerctl networkmanager-dmenu
```

> :diamonds: **oh-my-zsh & plugins**

- ```bash
  chsh -s /usr/bin/zsh # Change default shell to zsh for current user
  ```

- ```bash
  sh -c "$(wget https://raw.githubusercontent.com/robbyrussell/oh-my-zsh/master/tools/install.sh -O -)"
  ```

- ```bash
  git clone https://github.com/zsh-users/zsh-syntax-highlighting.git ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-syntax-highlighting
  ```

- ```bash
  git clone https://github.com/zsh-users/zsh-autosuggestions.git ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-autosuggestions
  ```

## :wrench: Dotfiles Install

> :file_folder: **General Config**

- ```bash
  git clone https://github.com/ilham25/dotfiles
  ```

- ```bash
  cd dotfiles/ && cp -r {.*,*} ~/
  ```

- ```bash
  rm -r ~/{README.md,LICENSE,.git} # Delete unnecessary files
  ```

> :nut_and_bolt: **Icons**

- ```bash
  cd ~/.icons/
  ```
- ```bash
  tar -Jxvf Papirus-Custom.tar.xz && tar -Jxvf Papirus-Dark-Custom.tar.xz
  ```

- ```bash
  sudo cp -r {Papirus-Custom,Papirus-Dark-Custom} /usr/share/icons/
  ```

- ```bash
  rm -r ~/.icons/{Papirus-Custom,Papirus-Dark-Custom,*.tar.xz} # Delete unnecessary files
  ```

> :bulb: **Refresh font cache**

```bash
fc-cache -rv
```

## :heart: Credits

- [i3wm Wiki](https://i3wm.org/docs/userguide.html)
- [@owl4ce](https://github.com/owl4ce/)
- [@nwg-piotr - psuinfo](https://github.com/nwg-piotr)
- [@horst3180 - Arch Theme](https://github.com/horst3180/arc-theme)
- [Persona Wallpaper](https://wall.alphacoders.com/big.php?i=756850)
