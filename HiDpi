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
xrandr --dpi 200
xrdb -merge ~/.Xresources
# ...
exec $@
```
``Xft.dpi`` should be ``200`` in ``.Xresource``.

For greeting screen, edit /etc/lightdm/lightdm-gtk-greeter.conf:

```
xft-dpi=200
```

Then restart to apply these settings:

```
systemctl restart lightdm
```
