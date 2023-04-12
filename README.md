# wallpapers
Wallpapers from various distros

## Gnome-backgrounds
URL `https://gitlab.gnome.org/api/v4/projects/1660/repository/tree?path=backgrounds&per_page=100`

```
let images = await fetch('https://gitlab.gnome.org/api/v4/projects/1660/repository/tree?path=backgrounds&per_page=100')
    .then(result => result.json())
    .then(result => result.map(obj => {
        if(obj.name.endsWith('.jpg') || obj.name.endsWith('.svg') || obj.name.endsWith('.webp'))
        return "https://gitlab.gnome.org/GNOME/gnome-backgrounds/-/raw/main/backgrounds/" + obj.name
    }));
```

## 
