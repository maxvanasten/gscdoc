# gscdoc

Welcome to `gscdoc`, my centralized repo for information about gsc scripting for older Call of Duty titles.

## Tools used

To find out information about gsc, I've been using my own tools that are specifically made for this purpose:

- [gscex](https://github.com/maxvanasten/gscex): A tui tool for searching through the original decompiled t5/t6 scripts.
- [gscp](https://github.com/maxvanasten/gscp): A parser for the gsc scripting language.
- [gsclsp](https://github.com/maxvanasten/gsclsp): A language server implementation for gsc using `gscp`. (Provides syntax highlighting, inline hints, jump-to-definition etc.)

# Index

<details>
<summary><h2>Common utility functions</h2></summary>

`common_scripts\utility` is a library script that is included in both T5 and T6. These functions can be used in either game identically. It is highly recommended to just `#include common_scripts\utility;` at the top of basically any script you make so you dont have to explicitly write that path out every time you want to use a utility function.
<details>
<summary><h3>Arrays</h3></summary>

| Function | Description | Documentation |
| -------- | ----------- | ------------- |
| `array(a,b,c,d...x,y,z)` | Create an array from up to 26 elements |  | 
| `add_to_array(arr, item, allowDupes)` | Add item to array | |
| `array_remove(arr, item)` | Remove item from array | |
| `random(arr)` | Returns random item from array | |
| `array_insert(arr, item, index)` | Add item to array at index | |
| `array_remove_index(arr, index)` | Remove item from array at index | |
| `array_delete(arr)` | Delete all elements from array | |
| `array_randomize(arr)` | Randomize array | |
| `array_reverse(arr)` | Reverse array | |
| `array_average(arr)` | Returns average value of array of numbers | |
| `array_removeundefined(arr)` | Removes undefined elements from array | |
| `array_combine(arr1, arr2)` | Combines two arrays | |
| `array_merge(arr1, arr2)` | Merges two arrays (Removes duplicated | |
| `is_in_array(arr, item)` | Returns `true` if element is in array | |
| `array_func(arr, func, arg1, arg2, arg3, arg4, arg5)` | Runs function on every item in array with up to 5 arguments | |
| `array_thread(arr, func, arg1, arg2, arg3, arg4, arg5)` | Runs threaded function on every item in array with up to 5 arguments | |
| `array_wait(arr, event, timeout)` | Wait for *every* item in array to receive notification | |
| `array_wait_any(arr, event, timeout)` | Wait for *any* item in array to receive notification | |
| `array_notify(arr, event)` | Notify every item in array of event | |
| `array_exclude(arr, arrExclude)` | Returns array minus items that are also present in arrExclude | |
</details>
<details>
<summary><h3>Flags</h3></summary>

| Function | Description | Documentation |
| -------- | ----------- | ------------- |
| `flag_init(flagName, value)` | Initializes flag with optional value | |
| `flag_set(flagName)` | Set flag on | |
| `flag_toggle(flagName)` | Toggle flag | |
| `flag_wait(flagName)` | Wait for flag | |
</details>
<details>
<summary><h3>Booleans</h3></summary>

| Function | Description | Documentation |
| -------- | ----------- | ------------- |
| `is_true(property)` | Check if property is not `undefined` and is `true` | |
| `is_false(property` | Check if property is not `undefined` and is `false` | |
</details>
</details>

<details>
<summary><h2>Zombies specific functions</h2></summary>
<details>
<summary><h3>Common (every map)</h3></summary>

| Function | Description | Documentation |
| -------- | ----------- | ------------- |
| `weapon_give(weaponName, isUpgrade, magicBox, noSound)` | Give weapon to player | |
| `give_perk(perkName, bought)` | Give perk to player | |
| `level.player_out_of_playable_area_monitor` | Enable/disable out of bounds check
</details>
</details>
