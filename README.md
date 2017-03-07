# XPS13-Manjaro
**Using community i3: https://manjaro.org/category/community-editions/i3/**

# TODO
- Add .conf files
- Clean .i3/config
- Fix rofi config
- Clean .i3/i3blocks.conf
- Disable Pc squeaky beep (PC speaker)  https://wiki.archlinux.org/index.php/PC_speaker


/usr/share/conky_solarized, i3blocks.conf, i3/conf


## Touchpad Configurations
Touchpad.md

## HiDpi Configuration
HiDpi.md

### Terminal Configuration (Zsh: oh-my-zsh)

- Install zsh 

```bash
pacman -S zsh
```
- Set zsh as default terminal shell 

```bash
chsh -s /bin/zsh
```

- From Oh-my-zsh github: https://github.com/robbyrussell/oh-my-zsh

```zsh 
cd && sh -c "$(curl -fsSL https://raw.githubusercontent.com/robbyrussell/oh-my-zsh/master/tools/install.sh)"
```
- Current theme: https://github.com/denysdovhan/spaceship-zsh-theme
- Terminal color scheme and font are under .Xresources. **tomorrow.dark** https://terminal.sexy

### Sublime Configuration
- Install package control: https://packagecontrol.io/installation
- Install base16 color scheme: https://github.com/chriskempson/base16-textmate
- Set color scheme to tomorrow-night
- Plugins:
  - SublimeLinter
  - SublimeLinter-contrib-eslint_d
  - SublimeLinter-pylint
  - SideBarEnhancements
  - Can I Use


