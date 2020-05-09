# Script: grive-status-polybar
Polybar module to display grive sync status

## Dependencies:
- [`Grive`](https://github.com/vitalif/grive2)
- A font that can display the characters `0xfb3e` and `0xf058`, I recommend a [Nerd Font](https://www.nerdfonts.com/). Although these can be changed in the script.

## Setup:
Change `FILE_EXPLORER` to your file explorer of choice and `DRIVE_DIR` to your Google Drive directory. If you place `grive-status.sh` somewhere else, don't forget to change the exec path.

## Module:
```ini
[module/grive-status]
type = custom/script
exec = ~/.local/bin/scripts/polybar/grive-status.sh
interval = 5
format = "<label>"
format-padding = 1

click-left = {FILE_EXPLORER} ~/{DRIVE_DIR}/ &
```
