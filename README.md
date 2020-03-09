# Genero Syntax Highlighting for VSCode

Highlighting for genero files with all the classic yellow and purples just as you remembered it.

Pairs best with [VSCodeVim](https://github.com/VSCodeVim/Vim) and [Remote Development](https://marketplace.visualstudio.com/items?itemName=ms-vscode-remote.vscode-remote-extensionpack).

## Features

Highlights syntax. That's about it for now.

## Requirements

Visual Studio Code I guess. Download the vsix file, hit F1, type in vsix and pick the install option. 
The default vsix extension will save genero files as .4gl by default. The one labelled cdn will save as .es.

You'll also need to add this to your settings.json file which you can find by pressing F1 and typing settings:

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
                    "foreground": "#d400ff"
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

Optionally, you can also add:

    "editor.renderIndentGuides": false,
    "vim.handleKeys": {
        "<C-x>": false,
        "<C-c>": false,
        "<C-v>": false,
        "<C-z>": false,
        "<C-y>": false,
        "<C-a>": false,
        "<C-s>": false
    }

This will remove the tab indent lines and get rid of some of the vim commands with the far more useful Windows ones.
If you like Ctrl-V in vim, middle click dragging in vscode does the same thing.

## Known Issues

There's probably a ton, but then again if they aren't known then they wouldn't be here anyways.

## Release Notes

### 07-03-2020 1.0.0

Initial release
