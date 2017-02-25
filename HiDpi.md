```zsh
lightdm --show-config
```

```
[Seat:*]
A  session-wrapper=/etc/lightdm/Xsession
```

Inject these 2 line above the end line exec $@ of file Xsession, so that it looks like:

```
# ...
xrandr --dpi 180
xrdb -merge ~/.Xresources
# ...
exec $@
```
``Xft.dpi`` should be ``180`` in ``~/.Xresources``.

For greeting screen, edit /etc/lightdm/lightdm-gtk-greeter.conf:

```
xft-dpi=180
```

Then restart to apply these settings:

```
systemctl restart lightdm
```
