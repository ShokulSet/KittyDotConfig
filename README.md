# Terminal Dotfiles

My personal terminal configuration — kitty, zsh, and oh-my-posh.

## Structure

```
.
├── kitty/               # Kitty terminal config
│   ├── kitty.conf       # Main config (font, window, opacity)
│   ├── current-theme.conf
│   ├── cyberdream.conf  # Default theme
│   ├── catppuccin-theme.conf
│   ├── oxocarbon.conf
│   ├── tokyonight_*.conf
│   └── toggle-transparency.sh
├── zsh/
│   └── .zshrc           # Zsh config with zinit, fzf, zoxide, vi-mode
└── oh-my-posh/
    ├── powerlevel10k-custom.yaml  # Active prompt theme
    └── robbyrussell.yaml
```

## Prerequisites

Install these via Homebrew:

```bash
brew install oh-my-posh fzf zoxide eza zsh-vi-mode
brew install --cask kitty
```

## Font

Uses [Maple Mono NF](https://github.com/subframe7536/maple-font) — install it first or change the font in `kitty.conf`.

## Kitty Setup

1. Copy all files from the root of this repo to `~/.config/kitty/`
2. To switch themes, edit `current-theme.conf`:
   ```
   include cyberdream.conf
   ```
3. Reload config: `cmd+ctrl+,`

## Zsh Setup

1. Copy `zsh/.zshrc` to `~/.zshrc`
2. Update any hardcoded paths (Flutter, Istio, etc.) to match your system
3. [zinit](https://github.com/zdharma-continuum/zinit) will auto-install on first launch

## Oh My Posh Setup

1. Copy `oh-my-posh/` files to `~/.config/oh-my-posh/themes/`
2. The active theme is `powerlevel10k-custom.yaml` (set in `.zshrc`)

## Toggle Transparency

```bash
chmod +x toggle-transparency.sh
./toggle-transparency.sh
```
