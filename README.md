# mpv mediaplayer snap with a main focus on Wayland support
\
Configuration files can be placed under `/home/<user>/snap/mpv-wayland/common/.config/mpv/` directory

___
### Enable youtube support:
```sh
snap install yt-dlp-core20  
snap connect mpv-wayland:plug20 yt-dlp-core20:yt-dlp-core20
```

___
### Allow access to /media, /run/media and /mnt:
```sh
snap connect mpv-wayland:removable-media
```

___
### Use KDE libs instead of Gnome:
```sh
snap install kde-frameworks-5-99-qt-5-15-7-core20
snap disconnect mpv-wayland:gnome-3-38-2004
snap connect mpv-wayland:gnome-3-38-2004 kde-frameworks-5-99-qt-5-15-7-core20:kde-frameworks-5-99-qt-5-15-core20
```
