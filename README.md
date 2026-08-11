# Interactive Solar System 🪐

An interactive 3D visualization of the Solar System built with [three.js](https://threejs.org/).
Open the single HTML file in any modern browser — no build step required.

**Live demo (GitHub Pages):** https://iosonolatte.github.io/interactive-solar-system/

## Run it

Just open `index.html` in a browser. three.js is loaded from a CDN via an import map,
so you need an internet connection on first load.

To serve it locally (optional):

```bash
# Python
python -m http.server 8000
# then visit http://localhost:8000/index.html
```

## Controls

| Action | How |
| --- | --- |
| Rotate view | Drag with mouse |
| Zoom | Scroll wheel |
| Inspect a body | Click the Sun, a planet, or a dwarf planet |
| Pause / play | Bottom control bar |
| Speed | Slider (default opening pace labeled `1.0×`) |
| Toggle orbits | Bottom control bar |
| Toggle labels | Bottom control bar |
| Reset view | Bottom control bar |

Clicking a body slides in an info card (diameter, distance from Sun, orbital/rotation period,
moon count, a fun fact) and the camera smoothly flies to and follows it.

## What's included

- **Sun** with emissive core, additive glow sprite, and `UnrealBloom` post-processing.
- **8 planets** with axial tilt, orbital inclination, and rings for Saturn & Uranus.
- **Earth's Moon** orbiting Earth.
- **Asteroid belt** between Mars and Jupiter (~2,400 particles).
- **5 dwarf planets** — Ceres (in the belt), Pluto, Haumea, Makemake, Eris (beyond Neptune).
- **Starfield** background (~6,000 stars).
- **CSS2D labels** with glowing pills, per-body color accents, and leader stems.

## Data accuracy

Body facts (diameters, orbital/rotation periods, moon counts, axial tilts) are grounded in the
[Wikipedia "Solar System"](https://en.wikipedia.org/wiki/Solar_System) article. The Sun holds
~99.86% of the system's mass and the system is ~4.6 billion years old.

⚠️ **Scale disclaimer:** planet **sizes and distances are display-scaled**, not true astronomical
scale — at real scale the planets would be invisible specks. Orbital *speeds* keep their real
relative ratios, so inner planets orbit noticeably faster than the outer ones.

## License

MIT — do whatever you like.
