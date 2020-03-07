# Genero Syntax Highlighting for VSCode

Highlighting for genero files with all the classic yellow and purples just as you remembered it.

## Features

Highlights syntax. That's about it for now.

## Requirements

Visual Studio Code I guess. You'll also need to add this to your settings.json file in 
C:/Users/*You*/AppData/Roaming/Code/User/:

    "editor.tokenColorCustomizations": {
        "textMateRules": [
            {
                "scope": "keyword.genero",
                "settings": {
                    "foreground": "#FFFF00"
                }
            },
            {
                "scope": "string.genero",
                "settings": {
                    "foreground": "#C99CFF"
                }
            },
            {
                "scope": "comment.genero",
                "settings": {
                    "foreground": "#00FFFF"
                }
            }
        ]
    }


## Known Issues

There's probably a ton, but then again if they aren't known then they wouldn't be here anyways.

## Release Notes

### 07-03-2020 1.0.0

Initial release

-----------------------------------------------------------------------------------------------------------


