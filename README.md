<h1 align="center">
  <img src="images/icon.png" alt="qualia-gtk-theme" width="156">
  <br>
  qualia-gtk-theme
</h1>

<p align="center"><b>
  This is the snap for <a href="https://github.com/dgsasha/dg-gnome-theme">qualia GTK theme</a></b>, <i>A Yaru and Libadwaita inspired theme designed to provide a consistent experience on GTK desktops</i>. 
</p>

<div align="center">

![dg-adw-gtk3-light](images/light.png?raw=true "dg-adw-gtk3-light")
![dg-adw-gtk3-dark](images/dark.png?raw=true "dg-adw-gtk3-dark")

</div>

## Install
```
sudo snap install qualia-gtk-theme
```

[![Get it from the Snap Store](https://snapcraft.io/static/images/badges/en/snap-store-white.svg)](https://snapcraft.io/qualia-gtk-theme)

[Don't have snapd installed?](https://snapcraft.io/docs/core/install)

## Enabling GTK3 Theme
```
for i in $(snap connections | grep gtk-common-themes:gtk-3-themes | awk '{print $2}'); do sudo snap connect $i qualia-gtk-theme:gtk-3-themes; done
```

## Enabling Icon Theme
```
for i in $(snap connections | grep gtk-common-themes:icon-themes | awk '{print $2}'); do sudo snap connect $i qualia-gtk-theme:icon-themes; done
```

## Enabling Sound Theme
```
for i in $(snap connections | grep gtk-common-themes:sound-themes | awk '{print $2}'); do sudo snap connect $i dqualia-gtk-theme:sound-themes; done
```