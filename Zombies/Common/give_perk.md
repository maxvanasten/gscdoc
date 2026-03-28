# give_perk()

Gives the player any perk.

## Description

This function handles all the side logic for correctly giving a player a perk.

## Signature

| Game | Function Call |
|------|---------------|
| t5 | `maps\_zombiemode_perks::give_perk(perkName, bought)` |
| t6 | `maps\mp\zombies\_zm_perks::give_perk(perkName, bought)` |

## Parameters

| Parameter | Type | t5 | t6 | Description |
|-----------|------|----|----|-------------|
| perkName | string | ✓ | ✓ | Name of the perk to give |
| bought | bool | ✓ | ✓ | Plays burp audio and blur effect |

## Return Value

| Game | Type | Description |
|------|------|-------------|
| t5 | void | No return value |
| t6 | void | No return value |

## Examples

### T5 (Black Ops)
```c
player thread maps\_zombiemode_perks::give_perk("specialty_armorvest", false);
```

### T6 (Black Ops II)
```c
player thread maps\mp\zombies\_zm_perks::give_perk("specialty_armorvest", false);
```
