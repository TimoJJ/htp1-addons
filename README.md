# htp1-addons

Addon catalog for the Monolith HTP-1. It holds only `index.json`; the
packages are attached to this repository's releases.

| Addon | What it is |
|---|---|
| `webui-alt` | Modified WebUI based on the stock HTP-1 WebUI. Optimized for desktop use with the light theme. When switched on, it replaces the WebUI at `/`; the stock UI remains available at `/ui/default`. |

## Install

On the HTP-1 web UI, open Settings, then Addons, and add this repository's
address:

```
https://github.com/TimoJJ/htp1-addons
```

The unit lists the addons from `index.json`, downloads the package from the
release, checks its SHA-256 and installs it. `webui-alt` is off after install;
turn its switch on to make it the web UI.
