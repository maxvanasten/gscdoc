# function_name

Brief one-line description of what the function does.

## Description

Expanded description with more context, use cases, and important details.

## Signature

| Game | Function Call |
|------|---------------|
| t5 | `path::function_name(param1, param2)` |
| t6 | `path::function_name(param1, param2, param3)` |

## Parameters

| Parameter | Type | t5 | t6 | Description |
|-----------|------|----|----|-------------|
| param1 | string | ✓ | ✓ | Description |
| param2 | int | ✓ | ✓ | Description |
| param3 | bool |  | ✓ | Description |

## Return Value

| Game | Type | Description |
|------|------|-------------|
| t5 | void | No return value |
| t6 | entity | Returns the created weapon entity |

## Examples

### T5 (Black Ops)
```c
player thread path::function_name("value", 0);
```

### T6 (Black Ops II)
```c
player thread path::function_name("value", 0, 1, 0);
```

## Notes

Editor's discretion for implementation details, warnings, and cross-references.
