# weapon_give

This function is an all-in-one function for giving the player any weapon in the zombies gamemode in t5 and t6

| Function | Game | Engine/File | (t5) arguments | (t6) arguments |
| -------- | ---- | ----------- | -------------- | -------------- |
| weapon_give | t5/t6 | t5: `common\maps\_zombiemode_weapons.gsc`, t6: `maps\mp\zombies\_zm_weapons.gsc` | weaponName, isUpgrade | weaponName, isUpgrade, magicBox, noSound |

## Function

t5: `common\maps\_zombiemode_weapons::weapon_give( weaponName, isUpgrade )`
t6: `maps\mp\zombies\_zm_weapons::weapon_give( weaponName, isUpgrade, magicBox, noSound )`

## Arguments

### [t5/t6] weaponName

`string`: Reference [weapons list](#)

### [t5/t6] isUpgrade

`1`: Apply pack a punch camo/attachments

### [t6] magicBox

`1`: Plays voice line

### [t6] noSound

`1`: Does NOT play "purchase" sound effect

## Usage

### t5
```c
player thread maps\_zombiemode_weapons::weapon_give( "m1911_zm", 0 );
```

### t6
```c
player thread maps\mp\zombies\_zm_weapons::weapon_give( "m1911_zm", 0, 0, 0);
```
