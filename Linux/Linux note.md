# Wifi
nmcli device wifi list
nmcli device wifi connect {name} password {password}
# Font
~/.local/share/fonts/
# SDDM
- SDDM theme: /usr/share/sddm/themes
- SDDM config: /etc/sddm/default.conf
# Xrandr
exec --no-startup-id xrandr --output eDP-1 --auto --primary --brightness 0.8 --output HDMI-1-1 --auto --left-of eDP-1