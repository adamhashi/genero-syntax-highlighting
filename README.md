# Genero Syntax Highlighting for VSCode

Highlighting for genero files with all the classic yellow and purples just as you remembered it.

Pairs best with [VSCodeVim](https://github.com/VSCodeVim/Vim) and [Remote Development](https://marketplace.visualstudio.com/items?itemName=ms-vscode-remote.vscode-remote-extensionpack).

## Features

Highlights syntax. That's about it for now.

## Requirements

Visual Studio Code I guess. Download the vsix file, hit F1, type in vsix and pick the install option. 
The default vsix extension will save genero files as .4gl by default. The one labelled cdn will save as .es.

You'll also need to add this to your settings.json file which you can find by pressing F1 and typing settings:

    "terminal.integrated.shellArgs.linux": ["-l"],
    "files.encoding": "windows1252",
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

The terminal setting lets vscode read your bash settings. Setting the encoding to Windows 1252 fixes errors
when working with files containing french characters.

Optionally, you can also add:

    "files.encoding": "windows1252",
    "git.untrackedChanges": "hidden",
    "editor.renderIndentGuides": false,
    "vim.handleKeys": {
        //"<C-x>": false,
    }

This will remove the tab indent lines. Add lines to vim.handleKeys if you want certain keyboard commands 
to default to the vscode function. The git setting hides untracked changes in the vscode source control page.

## Known Issues

There's probably a ton, but then again if they aren't known then they wouldn't be here anyways.

## Release Notes

### 05-May-2020 0.1.0

Removed autocomplete for IF/FOR blocks, fixed /* comments not highlighting

### 10-Mar-2020 0.0.2

Added highlighting for per elements

### 07-Mar-2020 0.0.1

Initial release
