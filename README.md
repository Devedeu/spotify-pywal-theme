# A pywal implementation for the default spotify theme
### How to install?
1. Install `pywal` and `spicetify` if you haven't already.
2. Download the `color.ini` from this repo and put it into `.config/wal/templates` and generate a colorscheme with pywal.
3. Create a folder for the theme in `.config/spicetify/Themes`. Ex: 
```
mkdir ~/.config/spicetify/Themes/defaultwal
```
It can be named anything, defaultwal is just for demonstration purposes

4. Create a symlink between the file in `.cache/wal` and the one in `.config/spicetify/Themes/defaultwal`

!!! The file in ~/.config/spicetify/Themes/defaultwal NEEDS to be named color.ini, otherwise it will not work! 

```
ln -s ~/.cache/wal/color.ini ~/.config/spicetify/Themes/defaultwal/color.ini
```
5. Apply the theme
```
spicetify config current_theme defaultwal
spicetify apply
```

where defaultwal is the name of the folder that was created in ~/.config/spicetify/Themes

6. Enjoy

## Reload script(Optional)

Since Spicetify won't update automatically whenever you generate a new colorscheme with pywal, a script needs to be used. You can make your own or use mine.

To use mine, download it, give it executable permission
```
chmod +x spicetifyupdater
```
and include it in your wal script or alias. I personally have it in my wallpaper changer script that can be found in my Dotfiles repo


# Showcase
https://github.com/user-attachments/assets/ad3c8bc0-5073-4360-8a2a-928e69330240
