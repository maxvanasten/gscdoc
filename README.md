# gscdoc

Welcome to `gscdoc`, my centralized repo for information about gsc scripting for older Call of Duty titles.

## Tools used

To find out information about gsc, I've been using my own tools that are specifically made for this purpose:

- [gscex](https://github.com/maxvanasten/gscex): A tui tool for searching through the original decompiled t5/t6 scripts.
- [gscp](https://github.com/maxvanasten/gscp): A parser for the gsc scripting language.
- [gsclsp](https://github.com/maxvanasten/gsclsp): A language server implementation for gsc using `gscp`. (Provides syntax highlighting, inline hints, jump-to-definition etc.)

# Index

<details>
<summary><h2>common_scripts\utility</h2></summary>

`common_scripts\utility` is a library script that is included in both T5 and T6. These functions can be used in either game identically.
<details>
<summary><h3>Arrays</h3></summary>

- [`array()`](): Create an array from up to 26 elements
- [`add_to_array()`](): Add item to array
- [`array_remove()`](): Remove item from array
- [`random()`](): Returns random element from array
- [`array_insert()`](): Add item to array at index
- [`array_remove_index()`](): Remove item from array at index
- [`array_delete()`](): Delete *all* elements from array
- [`array_randomize()`](): Randomize array
- [`array_reverse()`](): Reverse array
- [`array_average()`](): Returns the average number from array of numbers
- [`array_removeundefined()`](): Returns new array minus undefined elements
- [`array_combine()`](): Combines two arrays
- [`array_merge()`](): Combines two arrays, removes duplicate elements
- [`is_in_array()`](): Returns `true` if element is in array
- [`array_func()`](): Run a function on *every* element in an array
- [`array_thread()`](): Run a threaded function on *every* element in an array
- [`array_wait()`](): Wait for *every* entity in array to receive notification
- [`array_wait_any()`](): Wait for *any* entity in array to receive notification
- [`array_notify()`](): Notify *every* entity in array
- [`array_exclude()`](): Returns array minus elements that are also in exclusion list
</details>
<details>
<summary><h3>Flags</h3></summary>

- [`flag_init()`](): Initialize flag
- [`flag_set()`](): Set flag on
- [`flag_toggle()`](): Toggle flag on/off
- [`flag_wait()`](): Wait for flag
</details>
<details>
<summary><h3>Booleans</h3></summary>

- [`is_true()`](): Check if property is not `undefined` and is `true`
- [`is_false()`](): Check if property is not `undefined` and is `false`
</details>
</details>

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
