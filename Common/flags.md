# Flags

Flags are used to wait for custom events to happen before continuing the code.

## Description

There are a couple different important functions for working with flags. They are `flag_init`, `flag_set`, `flag_toggle`, `flag_wait`. These functions come from the `common_scripts\utility` script which has the same location for both t5 and t6. Flags *must* be initialized before use by doing `flag_init( "flag_name" );`. You can set the flag by using `flag_set( "flag_name" );` or toggle it if you want to reuse the flag by using `flag_toggle( "flag_name" );`. Then, anywhere else in your code you can wait for the flag to be set/toggled on by using `flag_wait( "flag_name" );`.

## Signatures

| Signature |
| --------- |
| common_scripts\utility::flag_init( flag_name ) |
| common_scripts\utility::flag_set( flag_name ) |
| common_scripts\utility::flag_toggle( flag_name ) |
| common_scripts\utility::flag_wait( flag_name ) |

## Example

```c
#include common_scripts\utility;

// Initialize the flag
flag_init("my_custom_flag");

// Set the flag
flag_set("my_custom_flag");
// OR: Toggle the flag
flag_toggle("my_custom_flag");

// Wait for flag to be set
flag_wait("my_custom_flag");
player iprintlnbold("my_custom_flag was triggered!");
```

## Notes

`flag_wait` automatically spawns a loop to check the flag, so you should not run `flag_wait` in an infinite loop yourself.
