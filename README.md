[![Board Status](https://dev.azure.com/hasifresearch/d3762b5a-7d19-43d0-8fbe-6bcb6430b952/46e6fad4-dbca-4477-9ae1-60ed2b0df7ca/_apis/work/boardbadge/4542d7d3-e8f0-4178-b0c9-54cc454875c3)](https://dev.azure.com/hasifresearch/d3762b5a-7d19-43d0-8fbe-6bcb6430b952/_boards/board/t/46e6fad4-dbca-4477-9ae1-60ed2b0df7ca/Microsoft.RequirementCategory)
<h1 align="center">my nord config</h1>

<div align="center">
Nord Themed Config File for i3-gaps, dunst, rofi, Alacritty, kitty, Zsh, neovim, Spotify, and many more<br>
  Inspired by this amazing color pattern https://nordtheme.com/<br>
<img src="https://github.com/jhagas/my-config/raw/main/Screenshot/3.png" width="763">
</div>

## Gnome/GTK/Kvantum Theme
Nordic: https://github.com/EliverLara/Nordic

## GTK Icons Theme
Papirus: https://github.com/PapirusDevelopmentTeam/papirus-icon-theme

## Installation
- ***First of all, clone this repository***
```bash
git clone https://github.com/jhagas/my-config
cd my-config
```

Everything should be in place as in this git repo.
Make sure `$HOME/.local/bin/` is on `$PATH`


### Chromium Startpage Install
1. Open Extensions menu on Chromium
2. Turn on developer mode
3. Click "Load Unpacked"
4. Find the startpage directory
usually located in
```~/my-config/startpage/```

### Spotify Theme Install
Make sure you already install Spicetify and have opened it before
```bash
cp -r Dribbliish ~/.config/spicetify/Themes/
```
Configuring:
```bash
cd "$(dirname "$(spicetify -c)")/Themes/Dribbblish"
mkdir -p ../../Extensions
cp dribbblish.js ../../Extensions/
spicetify config extensions dribbblish.js
spicetify config current_theme Dribbblish color_scheme nord-dark
spicetify config inject_css 1 replace_colors 1 overwrite_assets 1
spicetify apply
```
