# Kitty Terminal Config

My personal kitty terminal configuration.

## Files

| File | Description |
|------|-------------|
| `kitty.conf` | Main config (font, window, opacity, keymaps) |
| `current-theme.conf` | Points to the active theme |
| `cyberdream.conf` | Cyberdream theme (default) |
| `catppuccin-theme.conf` | Catppuccin Mocha theme |
| `oxocarbon.conf` | Oxocarbon theme |
| `tokyonight_night.conf` | Tokyo Night theme |
| `tokyonight_storm.conf` | Tokyo Night Storm theme |
| `tokyonight_moon.conf` | Tokyo Night Moon theme |
| `tokyonight_day.conf` | Tokyo Night Day theme |
| `toggle-transparency.sh` | Toggle background opacity on/off |

## Setup

1. Copy all files to `~/.config/kitty/`
2. To switch themes, edit `current-theme.conf` and change the `include` line:
   ```
   include cyberdream.conf
   ```
3. Reload kitty config with `ctrl+shift+f5` or `cmd+ctrl+,`

## Font

Uses [Maple Mono NF](https://github.com/subframe7536/maple-font) — install it first.

## Toggle Transparency

```bash
chmod +x toggle-transparency.sh
./toggle-transparency.sh
```
