# XPS13-Manjaro
**Using community i3: https://manjaro.org/category/community-editions/i3/**

## Touchpad Configurations

1. Packages to install: ``libinput-gestures, xdotool``
1. List devices and find touchpad id.

  ```zsh 
  xinput list | grep -i touchpad
  ```
1. Grab touchpad id, e.g: 
  ```↳ DLL0704:01 06CB:76AE Touchpad           	id=11	[slave  pointer  (2)] ```
1. List current configurations.
  
  ```zsh
   xinput list-props 11
  ```
1. Enable 2 finger and 3 finger click.
  
  ```zsh 
  xinput set-prop "DLL0704:01 06CB:76AE Touchpad" "libinput Click Method Enabled" 0 1
  ```
1. Enable tap to click.

  ```zsh
  xinput set-prop "DLL0704:01 06CB:76AE Touchpad" "libinput Tapping Enabled" 1
  ```
1. Enable natural scroll (mac like scroll).

   ```zsh
   xinput set-prop "DLL0704:01 06CB:76AE Touchpad" "libinput Natural Scrolling Enabled" 1
   ```
1. Accelarate pointer speed.

  ```zsh
  xinput set-prop "DLL0704:01 06CB:76AE Touchpad" "libinput Accel Speed" 1  
  ```
