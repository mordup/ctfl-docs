# Compatibility

CTFL works on any Linux desktop environment with system tray support.

## Desktop environments

| Desktop | Status |
|---|---|
| KDE Plasma | Works out of the box |
| XFCE | Works out of the box |
| Cinnamon | Works out of the box |
| MATE | Works out of the box |
| LXQt | Works out of the box |
| GNOME | Requires the [AppIndicator](https://extensions.gnome.org/extension/615/appindicator-support/) extension |
| Sway / i3 / Hyprland | Works with a bar that has tray support (waybar, polybar, etc.) |

## GNOME setup

GNOME doesn't include a system tray by default. To use CTFL on GNOME:

1. Install the [AppIndicator Support](https://extensions.gnome.org/extension/615/appindicator-support/) extension
2. Enable it in GNOME Extensions
3. Launch CTFL — it will appear in the top bar

## Tiling window managers

For Sway, i3, Hyprland, and similar:

- **Waybar**: Enable the `tray` module in your waybar config
- **Polybar**: Enable the `tray` module
- Other bars: Any bar with XEmbed or StatusNotifierItem tray support will work
