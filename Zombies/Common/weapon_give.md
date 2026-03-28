# weapon_give()

Gives the player a weapon with optional Pack-a-Punch upgrade and sound control.

## Description

This function is an all-in-one function for giving the player any weapon in the zombies gamemode. It handles weapon allocation, optional Pack-a-Punch upgrades (camo/attachments), and sound effects. Available in both T5 (Black Ops) and T6 (Black Ops II) versions.

## Signature

| Game | Function Call |
|------|---------------|
| t5 | `maps\_zombiemode_weapons::weapon_give(weaponName, isUpgrade)` |
| t6 | `maps\mp\zombies\_zm_weapons::weapon_give(weaponName, isUpgrade, magicBox, noSound)` |

## Parameters

| Parameter | Type | t5 | t6 | Description |
|-----------|------|----|----|-------------|
| weaponName | string | ✓ | ✓ | The weapon reference name (e.g., `"m1911_zm"`) |
| isUpgrade | int | ✓ | ✓ | Set to `1` to apply Pack-a-Punch camo and attachments |
| magicBox | int |  | ✓ | Set to `1` to play character voice line |
| noSound | int |  | ✓ | Set to `1` to suppress the "purchase" sound effect |

## Return Value

| Game | Type | Description |
|------|------|-------------|
| t5 | void | No return value |
| t6 | void | No return value |

## Examples

### T5 (Black Ops)
```c
player thread maps\_zombiemode_weapons::weapon_give("m1911_zm", 0);
```

### T6 (Black Ops II)
```c
player thread maps\mp\zombies\_zm_weapons::weapon_give("m1911_zm", 0, 0, 0);
```

## Notes

- This function should be called on a player entity
- The `isUpgrade` parameter determines whether the weapon receives Pack-a-Punch visual treatment
- In T6, `magicBox` voice lines are typically played when obtaining weapons from the Mystery Box
- Use `noSound` when giving weapons silently (e.g., initial loadout, scripted sequences)
- Both versions use `thread` to avoid blocking execution
