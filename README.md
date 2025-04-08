# msl-syntax-highlighter README

Work in progress syntax highlighter for the Midas Script Language

## Features

Simple syntax highlighting for .msl files

## Requirements

None

## Extension Settings

#### Include different stylings for LOOP and IF blocks

To include different styles for LOOP and IF blocks, one has to add custom stylings for those scopes to the user settings (Command Pallet -> Preferences: Open User Settings (JSON)).
Here include the following block at the end of you settings and adjust the color parameters to your liking.

``` json
"editor.tokenColorCustomizations": {
    "textMateRules": [
        {
            "scope": "keyword.control.conditional",
            "settings": {
                "foreground": "#e06c8f",
            }
        },
        {
            "scope": "keyword.control.loop",
            "settings": {
                "foreground": "#e06cd6",
            }
        }
    ]
},
```





## Release Notes

### 0.0.1

Initial release

### 0.0.2 

Enable for older VSCode Versions

### 0.0.3

Added further Keywords

#### 0.0.4 

Added odb save

#### 0.0.5 

Added further parameter variables

#### 0.0.6

Added some more builtin functions and parameters

#### 0.0.7

Updated README