# Best dpi for QHD+ XPS

```
xft-dpi=180
```

## Login Screen & X (Using Lightdm)

- Edit session-wrapper for lightdm. ``/etc/lightdm/Xsession``
- Add the following 2 lines above end line ``exec $@``.

```
# ...
xrandr --dpi 180
xrdb -merge ~/.Xresources
# ...
exec $@
```
- ``~/.Xresources`` should include ``Xft.dpi=180``.
- For greeting screen, add ``xft-dpi=180`` in ``/etc/lightdm/lightdm-gtk-greeter.conf``.
- Restart to apply:

```
systemctl restart lightdm
```

## Terminal Font and cursor

 - Under ``~/.Xresources``:
 
 ```
 Xcursor.theme: whiteglass
 Xcursor.size: 24

 URxvt.font: xft:DejaVu Sans Mono:size=10
 ```
