# Waybar integration

Add the module to your Waybar configuration and include it in the desired
module list:

```jsonc
{
  "modules-right": [
    "custom/niri-columns"
  ],
  "custom/niri-columns": {
    "exec": "niri-columns --inactive ○ --active ● --hide-single",
    "return-type": "json"
  }
}
```

Ensure `niri-columns` is on Waybar's `PATH`, for example by installing it in
`~/.local/bin`.

Style the module in your Waybar stylesheet with the
`#custom-niri-columns` selector.
