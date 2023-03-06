## mpv mediaplayer snap with a main focus on Wayland support

To use with KDE libs instead of Gnome:

```sh
snap install kde-frameworks-5-99-qt-5-15-7-core20
snap install mpv-wayland
snap disconnect mpv-wayland:gnome-3-38-2004
snap connect mpv-wayland:gnome-3-38-2004 kde-frameworks-5-99-qt-5-15-7-core20:kde-frameworks-5-99-qt-5-15-core20
```
