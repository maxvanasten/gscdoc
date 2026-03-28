# `is_true()`/`is_false()`

These are some very simple helper functions for asserting the value of a boolean safely.

## Description

Normally, if the engine checks a variable that does not exist, the game will crash. This means that we always have to check if variables are defined before checking them, this can be annoying to do explicitly so the original devs added very simple helper functions in the `common_scripts\utility` file. This functionality is the same in t5 and t6.

## Signature

| Signature |
| --------- |
| `common_scripts\utility::is_true(property)` |
| `common_scripts\utility::is_false(property)` |

## Parameters

| Parameter | Type | t5 | t6 | Description |
|-----------|------|----|----|-------------|
| property | property | ✓ | ✓ | Property to check for `true`/`false` |

## Return Value

| Game | Type | Description |
|------|------|-------------|
| t5 | boolean | Result of check |
| t6 | boolean | Result of check |

## Examples

### T5 (Black Ops)
```c
if (common_scripts\utility::is_true(player.some_prop)) {
    player iprintln("some_prop is true!");
}
```

### T6 (Black Ops II)
```c
if (common_scripts\utility::is_false(player.some_prop)) {
    player iprintln("some_prop is false!");
}
```
