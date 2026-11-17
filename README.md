# ClayOS 18

A self-contained, interactive polymer clay iOS 18 simulation built in a single zero-dependency HTML file ([clay_ios.html](./clay_ios.html)). Designed around hand-sculpted SVG textures, plasticine deformation physics, Web Audio synthesis, and an interactive craft workshop bench.

## Features

### 4-Page Clay Home Screen & OS Shell
- **Today View (`Page 1`)**: Live Weather, Calendar, Clay Orchestra (Music), Battery, and Pinned Note widgets.
- **Hero Home Screen (`Page 2`)**: 3×4 polymer clay icon grid with 4-seed relief/fingerprint textures, notification badges, sculpted Apple & `iOS 18` centerpiece, and a 4-app Dock (`Phone`, `Safari`, `Music`, `Photos`).
- **Studio & Utilities (`Page 3`)**: `Calculator`, `Reminders`, `Voice Memos`, `Clay Studio`, plus apps installed via the App Store.
- **App Library (`Page 4`)**: Categorized app grid and quick Spotlight launcher.
- **System Overlays & Hardware Controls**: Lock Screen, expandable Dynamic Island, Control Centre, Spotlight Search (`/` or `Ctrl`/`Cmd + K`), App Switcher, StandBy nightstand mode, Siri command palette, jiggle-mode icon reordering, and clickable side Volume, Lock, and customizable Action buttons.

### 19 Interactive Apps
- **Communication & Media**: `Messages` (threads + tapback reactions), `Mail`, `Phone` (keypad dialing + live Dynamic Island call state), `Photos`, `Camera`, `Music` (Web Audio synth playback + 4×8 beat sequencer), `Voice Memos`.
- **Productivity & Info**: `Calendar`, `Clock` (live analog dial), `Maps`, `Weather`, `Notes` (pinning + export), `Files` (browsing + inline previews), `Reminders`, `Calculator`, `App Store`, `Safari` (built-in clay pages + mini-game).
- **Creation & Customization**: `Clay Studio` and `Settings`.

### Polymer Clay Physics & Sculpting
- **Tactile Putty Physics (`#clayPhysics`)**: Icons squish directionally on press, nudge neighboring icons with radial ripples, and leave asymmetric 3D thumb craters on the wallpaper.
- **Persistent Sculpt Bar (`Sculpt` mode)**: Switch between **Thumb Dent**, **Roll Clay** (interpolated continuous clay coils), and extruded 3D clay charms (**`★`**, **`♥`**, **`✿`**) with `S` / `M` / `L` brush sizes and polymer swatches.
- **Workshop Toolbar**: Toggle **3D Tilt**, **Lamp** lighting, **Smooth** (clear craters/sculpt marks), Lock, Controls, Search, Switcher, Siri, and StandBy.

### Clay Customization Suite (`Clay Studio` & `Settings`)
- **Mix Clay Lab (`Clay Studio` → `Mix Clay Lab`)**: Blend any two polymer colors across a 0–100% knead ratio, save custom swatches, **Mold Phone Case**, **Dye Wallpaper**, **Marbleize Both** strata layers, or export **Sculpt Canvas** artwork as PNG.
- **Surface Finishes**: `Matte Bisque`, `Kiln Glaze`, and `Speckled Clay`.
- **Clay Compound Softness**: `Soft Putty`, `Classic Clay`, and `Kiln Baked` (adjusts deform stretch/tilt, neighbor ripple force, and crater persistence).
- **Polymer Case Presets**: `Natural Bisque`, `Terracotta`, `Sage Polymer`, `Lilac Dough`, `Charcoal Clay`, or your live `Custom Mix`.
- **Centerpiece & Bench Themes**: Customize the Apple & `iOS 18` centerpiece (`Bisque`, `24k Gold`, `Terracotta`, `Porcelain`, or `Hide`) and switch workshop surfaces (`Wood Bench`, `Cream Plaster`, `Kiln Slate`, `Cutting Mat`), also controllable via **Siri** voice commands.

## Running Locally

No build step or package installation is required—everything lives in `clay_ios.html`.

Serve the directory over HTTP (recommended so browser storage and media APIs work consistently) or open `clay_ios.html` directly:

```bash
python -m http.server 8418 --bind 127.0.0.1
```

Then open `http://127.0.0.1:8418/clay_ios.html` in a modern browser.

## Keyboard Shortcuts

- `/` or `Ctrl+K` / `Cmd+K` — Open Spotlight Search
- `Escape` — Collapse Dynamic Island, close active overlay, or exit active app
- `Enter` — Send/submit inside active inputs (`Messages`, `Calendar`, `Reminders`, `Safari`, `Siri`)

## Project Structure

```text
ClayOS/
├── clay_ios.html   # Complete single-file ClayOS 18 simulation (HTML, CSS, SVG, Canvas physics, Web Audio, JS)
├── README.md       # Project documentation
└── .gitignore      # Ignored local OS/editor files
```
