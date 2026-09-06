# niri-columns

A compact indicator for columns in niri's scrolling layout. It marks the
focused column and updates from niri's IPC event stream.

**Requirements:** `niri` and `jq`

## Demo

(right-side of the bar)

https://github.com/user-attachments/assets/0aa50832-bfd5-48ae-9eae-a4c6566069be

## Usage

```sh
niri-columns [--layout horizontal|vertical] [--inactive CHARACTER] [--active CHARACTER] [--hide-single] [--output=json|plain]
```

By default, output is JSON (used by Waybar custom modules). Use `--output=plain`
for line-oriented text output. Or [contribute](#integrations) a new output format!

| Option | Description |
| --- | --- |
| `--layout horizontal\|vertical` | Layout orientation. Default: `horizontal`. |
| `--inactive CHARACTER` | Indicator for an unfocused column. Default: `○`. |
| `--active CHARACTER` | Indicator for the focused column. Default: `●`. |
| `--hide-single` | Print no indicator when the workspace has zero or one column. |
| `--output=json\|plain` | Select output format. Default: `json`. |

## Integrations

- [Waybar](waybar/)

Integration examples for other bars are welcome. Add each example in its own
top-level directory and link it here. If an integration needs a new output
format, add it through `--output` in `niri-columns`.
