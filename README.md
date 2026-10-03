# htp1-addons

Addon catalog for the Monolith HTP-1. It holds only `index.json`; the
packages are attached to this repository's releases.

| Addon | What it is |
|---|---|
| `webui-alt` | Modified WebUI based on the stock HTP-1 WebUI. Optimized for desktop use with the light theme. When switched on, it replaces the WebUI at `/`; the stock UI remains available at `/ui/default`. |

## Install

On the HTP-1 WebUI, open Settings, then Addons, and add this repository's
address:

```
https://github.com/TimoJJ/htp1-addons
```

The unit lists the addons from `index.json`, downloads the package from the
release, checks its SHA-256 and installs it. `webui-alt` is off after install;
turn its switch on and refresh the web page to replace the stock WebUI.

<br>

## What `webui-alt` changes (as of version 1.0.1)

The main changes over the stock WebUI, as seen by the user:

### Visual design (optimized for desktop, light theme first)
- Consistent flat button style with soft shadows, a clear pressed state in both themes, and a single color rule: blue = main action, light gray = neutral, yellow = restart/partial reset, red = destructive, green = state only.
- Switches and radio buttons are status dots (gray ring when off, green dot when on) with large click targets that span the whole row.

### Home
- Larger volume digits, center-aligned status cards without frames, steady status card heights when the signal drops, and distinct icons per audio format.

### Channel Levels
- Sliders, step buttons, per-channel linking, reset all, a clickable speaker map with readable level values, and a reset button on every channel row (grayed out when the channel is already at 0 dB).

### Settings pages
- Inputs/Upmix: short one-line headers with full names as tooltips, no row stripes behind buttons.
- PEQ and Loudness: clear section headings and dividers, labels with colons, steadier layout.
- Calibration: duplicate Advanced PEQ Options section removed.
- Macros: one macro open at a time, "Unsaved" badge, and a code editor that sizes itself to its commands (up to 20 rows).
- Volume Setup: Default buttons are disabled when the value is already the default, and Minimum Volume's default is -99 dB so it fits the front-panel display.
- Personalize: the top bar stays in view while scrolling, and the Home preview follows the scroll and stops at the Settings section.
