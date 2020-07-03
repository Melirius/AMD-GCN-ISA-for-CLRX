# AMD GCN ISA

This extension provides a basic language support for the AMD GCN instruction set architecture, especially suitable for [CLRadeonExtender assembler](https://github.com/CLRX/CLRX-mirror). This is based on the [work](https://marketplace.visualstudio.com/items?itemName=dbaumeis.amd-gcn-isa) of Dominik Baumeister.

## Features

For files with the extensions
- .isa
- .isa.txt
- .il
- .il.txt

the following tokens are emitted:
- `storage.type.amd-gcn-isa`
- `keyword.vector.amd-gcn-isa`
- `keyword.scalar.amd-gcn-isa`
- `keyword.control.label.amd-gcn-isa`
- `support.variable.vector.amd-gcn-isa`
- `support.variable.scalar.amd-gcn-isa`
- `comment.line.double-slash.amd-gcn-isa`
- `constant.numeric.float.amd-gcn-isa`
- `constant.numeric.integer.amd-gcn-isa`

For a starting point it is recommended to add the following code snippet to your theme (on Windows it is in %APPDATA%\Code\User\settings.json file):

```json
    "editor.tokenColorCustomizations":{
        "textMateRules": [
            {
                "scope": "constant.string.amd-gcn-isa",
                "settings": {
                    "foreground": "#a76c00"
                }
            },
            {
                "scope": "storage.type.amd-gcn-isa",
                "settings": {
                    "foreground": "#CC3333"
                }
            },
            {
                "scope": "keyword.vector.amd-gcn-isa",
                "settings": {
                    "foreground": "#33CCCC"
                }
            },
            {
                "scope": "keyword.scalar.amd-gcn-isa",
                "settings": {
                    "foreground": "#CC33CC"
                }
            },
            {
                "scope": "support.variable.vector.amd-gcn-isa",
                "settings": {
                    "foreground": "#CCCC33"
                }
            },
            {
                "scope": "support.variable.scalar.amd-gcn-isa",
                "settings": {
                    "foreground": "#6495ED"
                }
            },
            {
                "scope": "keyword.control.label.amd-gcn-isa",
                "settings": {
                    "foreground": "#33CC33"
                }
            },
            {
                "scope": "keyword.clrx.amd-gcn-isa",
                "settings": {
                    "foreground": "#999999"
                }
            }
        ]
    }
```

## Release Notes

### 1.0.0
Initial [release](https://marketplace.visualstudio.com/items?itemName=dbaumeis.amd-gcn-isa) by Dominik Baumeister.
### 1.0.1
Extension to different types of commands and comments by Ivan Siutsou.

## License

This extension is under the MIT license. See [License](https://github.com/GPUOpen-Tools/vscode-extensions/blob/master/LICENSE) file for full license information.