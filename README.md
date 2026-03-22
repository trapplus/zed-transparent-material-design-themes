# Material Prism

A collection of translucent dark themes for [Zed](https://zed.dev) with frosted glass blur, built on the [Material Design 3](https://m3.material.io/styles/color/system/overview) color system.

Originally based on [dark-glass-theme](https://github.com/magnuspladsen/dark-glass-theme) by Magnus Pladsen (which itself is based on Zedokai by slymax).

## Variants

| Name | Background tint |
|---|---|
| Material Prism | Neutral dark |
| Material Prism - Pink | Warm rose |
| Material Prism - Indigo | Deep blue |
| Material Prism - Teal | Cool green |
| Material Prism - Amber | Warm amber |
| Material Prism - Deep Purple | Rich violet |
| Material Prism - Blue Grey | Cool grey |
| Material Prism - Brown | Warm brown |

## Setup

The theme works out of the box in Zed, but to get the frosted glass blur effect you need a compositor that supports it.

### Hyprland

Add to your `hyprland.conf`:

```ini
decoration {
    blur {
        enabled = true
        size = 8
        passes = 2
        ignore_opacity = true
        new_optimizations = true
        xray = false
    }
}
```

Make sure `no_blur` is not applied globally to all windows. If you use a dots config like [end-4/dots-hyprland](https://github.com/end-4/dots-hyprland), comment out the line:

```ini
# windowrule = match:class .*, no_blur on
```

### KDE Plasma

Enable **Blur** in System Settings → Desktop Effects → Blur.

## Installation

Search for **Material Prism** in the Zed extension marketplace, or add manually to `~/.config/zed/settings.json`:

```json
{
  "theme": "Material Prism - Deep Purple"
}
```

## Credits

- [Magnus Pladsen](https://github.com/magnuspladsen) — original dark-glass-theme
- [slymax](https://github.com/slymax) — Zedokai (original base theme)
- [trapplus](https://github.com/trapplus) — Material Design 3 adaptation