# Installation

## Dependencies

### **Arch Linux**

> > For AUR helper, im using **yay**

> **i3 Windows Manager**

```bash
sudo pacman -S i3-gaps
```

> **Audio**

```bash
sudo pacman -S alsa-utils pulseaudio
```

> **Brightness**

```bash
yay -S brightnessctl
```

> **Network Monitor & RAM Usage**

```bash
yay -S psuinfo
```

> **Other utility (panel, notification, terminal, file manager, etc)**

```bash
yay -S dunst tint2 gsimplecal rofi feh lxappearance qt5ct qt5-styleplugins lxsession xautolock rxvt-unicode-patched xclip scrot thunar thunar-archive-plugin thunar-media-tags-plugin thunar-volman tumbler w3m geany nano vim viewnior pavucontrol parcellite neofetch htop picom gtk2-perl zsh zsh-completions imagemagick playerctl networkmanager-dmenu
```

> **oh-my-zsh & plugins**

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

## Dotfiles Install

> **General Config**

- ```bash
  git clone https://github.com/ilham25/dotfiles
  ```

- ```bash
  cd dotfiles/ && cp -r {.*,*} ~/
  ```

- ```bash
  rm -r ~/{README.md,LICENSE,.git} # Delete unnecessary files
  ```

> **Icons**

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

## Credits

- [i3wm Wiki](https://i3wm.org/docs/userguide.html)
- [Harry Elric](https://github.com/owl4ce/)
- [nwg-piotr - psuinfo](https://github.com/nwg-piotr)
- [horst3180 - Arch Theme](https://github.com/horst3180/arc-theme)
- [Persona Wallpaper](https://wall.alphacoders.com/big.php?i=756850)

```

```

```

```
