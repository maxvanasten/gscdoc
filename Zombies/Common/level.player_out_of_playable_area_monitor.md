# level.player_out_of_playable_area_monitor

This property controls wether or not the game checks if the player is out of bounds.

# Description

if true, the player will be killed instantly. Most maps have progressive playable area zones that expand when doors are opened etc, so if you want to allow the player to be out of that area (ie if you want to spawn a player in the crazy place on origins) you set this property to false.


## Property

| Game | Property |
|------|---------------|
| t5 | `level.player_out_of_playable_area_monitor` |
| t6 | `level.player_out_of_playable_area_monitor` |

## Examples

### T5 (Black Ops)
```c
level.player_out_of_playable_area_monitor = true;
```

### T6 (Black Ops II)
```c
level.player_out_of_playable_area_monitor = true;
```
