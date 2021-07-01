# VS Code Settings

## Font
* [Ubuntu Mono](https://fonts.google.com/specimen/Ubuntu+Mono)
* [Anonymous Pro](https://www.marksimonson.com/fonts/view/anonymous-pro)

## Themes/Color
* [One Monokai Theme](https://marketplace.visualstudio.com/items?itemName=azemoh.one-monokai)
* [Material Icon Theme](https://marketplace.visualstudio.com/items?itemName=PKief.material-icon-theme)

## IntelliSense/AutoComplete
* [Path Intellisense](https://marketplace.visualstudio.com/items?itemName=christian-kohler.path-intellisense)

## Styles/Formatting
* [ESLint](https://marketplace.visualstudio.com/items?itemName=dbaeumer.vscode-eslint)

## Settings

```json
{
    "workbench.startupEditor": "none",
    "window.zoomLevel": 0.5,
    "workbench.colorTheme": "One Monokai",
    "workbench.preferredLightColorTheme": "Atom One Light",
    "workbench.preferredDarkColorTheme": "One Monokai",
    "workbench.iconTheme": "material-icon-theme",
    "editor.fontFamily": "Ubuntu Mono, monospace",
    "editor.fontSize": 20,
    "editor.fontWeight": "500",
    "terminal.integrated.fontFamily": "Ubuntu Mono, monospace",
    "terminal.integrated.fontSize": 18,
    "terminal.integrated.fontWeight": "500",
    "editor.fontLigatures": false,
    "files.autoSave": "afterDelay",
    "launch": {
        "configurations": [
            {
                "type": "pwa-node",
                "name": "Launch Program",
                "program": "${file}",
                "request": "launch",
                "skipFiles": [
                    "<node_internals>/**"
                ]
            }
        ]
    }
}
```
