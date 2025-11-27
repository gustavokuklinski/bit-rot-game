# Bit Rot Game Builds

## Summary

* (Download)[##-Download]
* (Game Requirements)[##-Game-requirements]
* (For linux)[##-For-linux]
* (Game Controls)[##-Game-controls]
* (For modding and mapping)[##-For-modding-and-mapping]
* (Version and compilation details)[##-Version-and-compilation-details]

## Download
**Build only avaiable for Linux**

[FREE DOWNLOAD]() (without source code)

[BUY ON ITCH](https://gustavokuklinski.itch.io/bit-rot) (with source code)

**Help the developer**

[DONATIONS](https://ko-fi.com/gustavokuklinski) (ko-fi)
_Donations up to 5 USD can request a copy of the game with source code_

## Game requirements

OS: Linux x86_64
RAM: 1GB
DSK: 100MB
CPU: i3 (4th)

## For linux

```shell
$ ./bit-rot_linux # Open the game
$ ./editor_linux # Game editor
```

## Game controls

- **W/A/S/D**: Walk
- **SHIFT + W/A/S/D**: Run
- **CTRL/R-Click + L-Click**: Shoot/Attack
- **SHIFT + L-Click + Drag**: Get only one item from stack
- **L-Click + Drag**: Place or Drop
- **R-Click**: Opens context menu 
- **1/2/3/4/5**: Equip and use item from Belt
- **SPACE**: Wake up from sleep

- **E**: Get item from floor, open/close door
- **R**: Reload weapon

- **I**: Opens Inventory
- **H**: Open Status
- **N**: Open Nearby
- **M / ENTER**: Open Messages (enter enable chat mode)
- **G**: Open Clothes

- **F2 / ESC**: Pause, save, back to menu

- **MOUSE SCROLL**: Zoom in/Zoom out
- **-/=**: Keyboard Zoom in/Zoom out


## For modding and mapping

Basic structured codding: ```game/lib/data```: XML; ```game/save/game/[TIMESTAMP_DIR/]```: JSON
Basic excel (if needed for mapping): ```game/lib/map```: CSV
Designing: ```game/lib/sprites```: PNG

```game/``` Game folder have all game assets XML (map and items), CSV (map raw data), JSON (save files) and PNG (tiles and sprites)

Sprite size: 14x14px

**Folder structure**

```bash
└── game
    ├── icons
    ├── lib
    │   ├── data
    │   │   ├── clothes
    │   │   ├── items
    │   │   ├── language
    │   │   ├── map
    │   │   ├── player
    │   │   └── zombie
    │   ├── font
    │   ├── map
    │   ├── sfx
    │   │   ├── items
    │   │   ├── map
    │   │   ├── player
    │   │   └── zombie
    │   └── sprites
    │       ├── clothes
    │       ├── editor
    │       ├── items
    │       ├── map
    │       ├── player
    │       ├── ui
    │       └── zombie
    └── save
        ├── config
        ├── game
        └── player
```

## Version and compilation details
**Python**: 3.12.3
**PIP**: 
altgraph                  0.17.4
Faker                     37.12.0
Nuitka                    2.8.6
ordered-set               4.1.0
packaging                 25.0
pip                       24.0
pygame-ce                 2.5.6
pyinstaller-hooks-contrib 2025.9
setuptools                80.9.0
tzdata                    2025.2
zstandard                 0.25.0

**Version**: DEV