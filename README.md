# VS Code Settings

## Programming Languages Support
* [C/C++](https://marketplace.visualstudio.com/items?itemName=ms-vscode.cpptools)
* [C#](https://marketplace.visualstudio.com/items?itemName=ms-dotnettools.csharp)
* [Python](https://marketplace.visualstudio.com/items?itemName=ms-python.python)

## Font
* [Ubuntu Mono](https://fonts.google.com/specimen/Ubuntu+Mono)
* [Anonymous Pro](https://www.marksimonson.com/fonts/view/anonymous-pro)

## Themes/Color
* [One Monokai Theme](https://marketplace.visualstudio.com/items?itemName=azemoh.one-monokai)
* [Material Icon Theme](https://marketplace.visualstudio.com/items?itemName=PKief.material-icon-theme)

## IntelliSense/AutoComplete
* [Path Intellisense](https://marketplace.visualstudio.com/items?itemName=christian-kohler.path-intellisense)
* [Tailwind CSS Intellisense](https://marketplace.visualstudio.com/items?itemName=bradlc.vscode-tailwindcss)
* [styled-jsx](https://marketplace.visualstudio.com/items?itemName=blanu.vscode-styled-jsx)

## Styles/Formatting
* [ESLint](https://marketplace.visualstudio.com/items?itemName=dbaeumer.vscode-eslint)
* [Vue Language Features (Volar)](https://marketplace.visualstudio.com/items?itemName=Vue.volar)

## Settings

```json
{
    "workbench.startupEditor": "none",
    "workbench.preferredLightColorTheme": "Atom One Light",
    "workbench.colorTheme": "One Monokai",
    "workbench.preferredDarkColorTheme": "One Monokai",
    "workbench.iconTheme": "material-icon-theme",
    "window.zoomLevel": 0.5,
    "editor.fontFamily": "Ubuntu Mono, monospace",
    "editor.fontSize": 20,
    "editor.fontWeight": "500",
    "terminal.integrated.fontFamily": "Ubuntu Mono, monospace",
    "terminal.integrated.fontSize": 18,
    "terminal.integrated.fontWeight": "500",
    "editor.fontLigatures": false,
    "editor.unicodeHighlight.ambiguousCharacters": false,
    "liveServer.settings.donotShowInfoMsg": true,
    "files.autoSave": "afterDelay",
    "launch": {
        "configurations": [
            {
                "type": "node",
                "name": "Mocha Tests",
                "program": "${workspaceFolder}/node_modules/mocha/bin/_mocha",
                "request": "launch",
                "args": [
                    "-u",
                    "bdd",
                    "--timeout",
                    "999999",
                    "--colors",
                    "${file}"
                ],
                "internalConsoleOptions": "openOnSessionStart",
                "skipFiles": [
                    "<node_internals>/**"
                ]
            },
            {
                "type": "node",
                "name": "Launch Program",
                "program": "${file}",
                "request": "launch",
                "skipFiles": [
                    "<node_internals>/**"
                ],
                "console": "integratedTerminal"
            }
        ]
    },
    "[python]": {
        "editor.formatOnType": true
    },
}
```
