# [Tokyo Night](https://marketplace.visualstudio.com/items?itemName=enkia.tokyo-night)
A clean, dark Visual Studio Code theme that celebrates the lights of Downtown [Tokyo at night.](https://www.google.com/search?q=tokyo+night&newwindow=1&sxsrf=ACYBGNRiOGCstG_Xohb8CgG5UGwBRpMIQg:1571032079139&source=lnms&tbm=isch&sa=X&ved=0ahUKEwiayIfIhpvlAhUGmuAKHbfRDaIQ_AUIEigB&biw=1280&bih=666&dpr=2) 

**Note:** Many UI elements are intentionally low contrast so as not to distract. I can provide [customization settings](https://code.visualstudio.com/api/references/theme-color) similar to what is shown below to anyone who needs specific text brightened. 

## Screenshots
Tokyo Night
![Screenshot - Tokyo Night](https://raw.githubusercontent.com/enkia/tokyo-night-vscode-theme/master/static/ss_tokyo_night.png)

Tokyo Night Storm
![Screenshot - Tokyo Night Storm](https://raw.githubusercontent.com/enkia/tokyo-night-vscode-theme/master/static/ss_tokyo_night_storm.png)

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


## iTerm Theme
`tokyo-night.itermcolors` is supplied in this theme's ~/.vscode/extensions folder or via [github.](https://github.com/enkia/tokyo-night-vscode-theme/blob/master/tokyo-night.itermcolors)   

**Enjoy!**
    
    
    


Tokyo Tower icon used in theme icon made by Smashicons from www.flaticon.com
