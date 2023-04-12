# wallpapers
Wallpapers from various distros

## gnome-backgrounds
* URL https://gitlab.gnome.org/api/v4/projects/1660/repository/tree?path=backgrounds&per_page=100
* REPO https://gitlab.gnome.org/GNOME/gnome-backgrounds
* LICENSE https://gitlab.gnome.org/GNOME/gnome-backgrounds/-/blob/main/COPYING

```
let images = await fetch('https://gitlab.gnome.org/api/v4/projects/1660/repository/tree?path=backgrounds&per_page=100')
    .then(result => result.json())
    .then(result => result.map(obj => {
        if(obj.name.endsWith('.jpg') || obj.name.endsWith('.svg') || obj.name.endsWith('.webp'))
        return "https://gitlab.gnome.org/GNOME/gnome-backgrounds/-/raw/main/backgrounds/" + obj.name
    }));
```

## manjaro-wallpapers
* URL https://gitlab.manjaro.org/artwork/wallpapers

## Debian wallpapers
* URL https://wiki.debian.org/DebianDesktop/Artwork#Artwork_Releases

## Budgie Desktop Wallpapers
* URL https://github.com/UbuntuBudgie/budgie-wallpapers
