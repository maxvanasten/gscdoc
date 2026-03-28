# gscdoc

Welcome to `gscdoc`, my centralized repo for information about gsc scripting for older Call of Duty titles.

## Tools used

To find out information about gsc, I've been using my own tools that are specifically made for this purpose:

- [gscex](https://github.com/maxvanasten/gscex): A tui tool for searching through the original decompiled t5/t6 scripts.
- [gscp](https://github.com/maxvanasten/gscp): A parser for the gsc scripting language.
- [gsclsp](https://github.com/maxvanasten/gsclsp): A language server implementation for gsc using `gscp`. (Provides syntax highlighting, inline hints, jump-to-definition etc.)

# Index

- Common
    - [Flags](./Common/flags.md): Initialize, set, toggle and wait for flags
- Multiplayer
    - Common
    - Maps
- Singleplayer
    - Common
    - Maps
- Zombies
    - Common
        - [`weapon_give()`](./Zombies/Common/weapon_give.md): Give the player any weapon
        - [`give_perk()`](./Zombies/Common/give_perk.md): Give the player any perk
        - [`level.player_out_of_playable_area_monitor`](./Zombies/Common/level.player_out_of_playable_area_monitor.md): Enable/Disable out of bounds check
    - Maps
