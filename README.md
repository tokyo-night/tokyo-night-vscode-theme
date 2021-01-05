# [Tokyo Night](https://marketplace.visualstudio.com/items?itemName=enkia.tokyo-night)
[![Version](https://vsmarketplacebadge.apphb.com/version/enkia.tokyo-night.svg)](https://marketplace.visualstudio.com/items?itemName=enkia.tokyo-night)
[![Rating](https://vsmarketplacebadge.apphb.com/rating-star/enkia.tokyo-night.svg)](https://marketplace.visualstudio.com/items?itemName=enkia.tokyo-night)
[![Issues](https://img.shields.io/github/issues/enkia/tokyo-night-vscode-theme)](https://github.com/enkia/tokyo-night-vscode-theme/issues)
<br><br>A clean, dark (and now light) Visual Studio Code theme that celebrates the lights of Downtown [Tokyo at night.](https://www.google.com/search?q=tokyo+night&newwindow=1&sxsrf=ACYBGNRiOGCstG_Xohb8CgG5UGwBRpMIQg:1571032079139&source=lnms&tbm=isch&sa=X&ved=0ahUKEwiayIfIhpvlAhUGmuAKHbfRDaIQ_AUIEigB&biw=1280&bih=666&dpr=2) 
<br><br>**Note:** Many UI elements are intentionally low contrast so as not to distract. I can provide [customization settings](https://code.visualstudio.com/api/references/theme-color) similar to what is shown below to anyone who needs specific text brightened. 
<br><br>**Visual Studio Code 1.48.1 change to console.log:** They [removed the special text mate rule for console.log](https://github.com/microsoft/vscode/issues/104616#issuecomment-675066291) so there is currently no way to distinguish it from a regular object / method aside from using eslint.
<br><br>**Visual Studio Code 1.43.0 change to syntax highlighting:** This theme currently (in my opinion) works best with semantic syntax highlighting turned off. To disable the feature, search for or add this to your settings:
```javascript
"editor.semanticHighlighting.enabled": false
```

## Screenshots
Tokyo Night
![Screenshot - Tokyo Night](https://raw.githubusercontent.com/enkia/tokyo-night-vscode-theme/master/static/ss_tokyo_night.png)

Tokyo Night Storm
![Screenshot - Tokyo Night Storm](https://raw.githubusercontent.com/enkia/tokyo-night-vscode-theme/master/static/ss_tokyo_night_storm.png)

Tokyo Night Light
![Screenshot - Tokyo Night Light](https://raw.githubusercontent.com/enkia/tokyo-night-vscode-theme/master/static/ss_tokyo_day.png)

## Disabling Italics
Paste this into your [settings.json](https://code.visualstudio.com/docs/getstarted/settings#_settings-file-locations) to disable italics.

```javascript
"editor.tokenColorCustomizations": {
    "[Tokyo Night]": { // or "[Tokyo Night Storm]"
        "textMateRules": [{
            "scope": [
                "comment",
                "meta.var.expr storage.type",
                "keyword.control.flow",
                "meta.directive.vue punctuation.separator.key-value.html",
                "meta.directive.vue entity.other.attribute-name.html",
                "tag.decorator.js entity.name.tag.js",
                "tag.decorator.js punctuation.definition.tag.js",
                "storage.modifier"
            ],
            "settings": {
                "fontStyle": ""
            }
        }]
    }
}
```

## Brightening Codelens text
I prefer my Codelens text fade into the background unless hovered over, but if you'd like a higher contrast, add this to your settings.json:
```javascript
"workbench.colorCustomizations": {
    "[Tokyo Night]": { // or "[Tokyo Night Storm]"
        "editorCodeLens.foreground": "#7982a9", // Preferred hex color
    }
}
```

## Window Active and Inactive borders (vscode 1.40.0)
macOS dark-mode doesn't play well with these two theme mods so I've chosen to darken them as much as I can to fix the gray border issue on my side. Set them however you like using:
```javascript
"workbench.colorCustomizations": {
    "[Tokyo Night]": { // or "[Tokyo Night Storm]"
        "window.activeBorder": "#ff0000",
        "window.inactiveBorder":"#0000ff"
    }
}
```


## Other portings
**iTerm**  
`tokyo-night.itermcolors` is supplied in this theme's ~/.vscode/extensions folder or via [github.](https://github.com/enkia/tokyo-night-vscode-theme/blob/master/tokyo-night.itermcolors)

**Sublime Text**  
*Tokyo Night* is a color scheme option in my [Enki Theme.](https://packagecontrol.io/packages/Enki%20Theme)

**DuckDuckGo**
[DuckduckGo theme preferences](https://duckduckgo.com/?kae=d&ks=m&kak=-1&kax=-1&kaq=-1&kap=-1&kao=-1&kau=-1&k5=1&k7=1a1b26&kj=16161e&kx=1abc9c&k21=16161E&k18=-1&ka=e&kaa=BB9AF7&k9=C0CAF5&k8=6183BB&kt=e)

**Jetbrains IDE**
[Tokyo Night Color Scheme](https://plugins.jetbrains.com/plugin/15662-tokyo-night-color-scheme) works best with material theme plugin and [this theme](https://github.com/Grafikart/tokyo-night-jetbrains-theme/blob/main/tokyonight.xml)

**Alfred**   
Install the [Tokyo Night Alfred Theme.](https://www.alfredapp.com/extras/theme/puSaeqbft2/)

**kitty terminal**  
[Tokyo Night kitty theme](https://github.com/davidmathers/tokyo-night-kitty-theme) is a color scheme for [kitty](https://sw.kovidgoyal.net/kitty/).

** VIM\/Neovim **
[tokyonight.vim](https://github.com/ghifarit53/tokyonight-vim), a [VIM](https://www.vim.org/)/[Neovim](https://neovim.io/) color scheme.  
This theme also has support for [lightline](https://github.com/itchyny/lightline.vim) as well as [airline](https://github.com/vim-airline/vim-airline).

**Alacritty Terminal**
[Tokyo Night Alacritty Theme](https://github.com/zatchheems/tokyo-night-alacritty-theme), a color scheme for [Alacritty Terminal Emulator](https://github.com/alacritty/alacritty)

<br><br>
**Enjoy!**

###### Tokyo Tower icon used in theme icon made by Smashicons from www.flaticon.com
