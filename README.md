# 🌀 Dreamwalker 3D

A surreal, open-world 3D dream game that runs entirely in your browser. You wake at the edge of a vast, quiet city. Six ruins hold the pieces of something you lost. Fly over the skyline, step through pink portals, talk to the few who stayed, and find your way to the spire at the center.

**No build step. No dependencies to install.** One `index.html` and [Three.js](https://threejs.org/) loaded from a CDN.

## ▶️ Play

https://dreamwalkerio.vercel.app/

## 🎮 Controls

| Action | Desktop | Mobile |
|---|---|---|
| Walk | `W` `A` `S` `D` | On-screen joystick |
| Orbit camera | Click + drag | Touch + drag |
| Float up / fly | Hold `Space` | ▲ button |
| Sink | Hold `Shift` | ▼ button |
| Talk to someone | `E` | Tap the "talk" prompt |
| Close dialog | `Esc` | Tap the button |

## 🧩 How to play

1. Walk (or fly) to the **six glowing gold pillars** scattered across the city. Each is a dream: choose how to respond and you recover a **fragment**, saved to your Journal.
2. Talk to the **blue-white figures** who stayed behind. Each has a few lines that cycle as you return.
3. Once all six fragments are found, the **spire at the city's center** lights up. Walk into it for the ending.
4. Step through the **pink portal rings** to be thrown across the map. Land on rooftops. Watch the sky.

## ✨ Features

- Procedurally laid-out city (40 × 30 blocks) with zoned districts: glass towers downtown, brick mid-rises, low warehouses on the outskirts, and a plaza with trees and a fountain
- Instanced rendering (hundreds of buildings, windows, signs) for smooth performance
- Third-person player with a visible character and orbit camera
- Free flight with solid, landable rooftops
- Full day/night cycle with a sun, drifting clouds, and a starlit gradient sky
- Rain, dust, birds, rising lanterns, wandering shades, and talkable NPCs
- Surreal sky: ringed planet, watching eyes, sky whales, aurora, floating inverted towers
- Neon signs that ripple through the rainbow, and periodic "dream shifts" (hue storms, floaty gravity, warped FOV)
- Touch controls for mobile

## 🛠️ Customize

Everything is in `index.html`. Useful knobs near the top of the script:

| What | Where |
|---|---|
| City size | `COLS`, `ROWS`, `CELL` |
| Dream scenes, choices, and fragments | `DREAMS` object |
| NPC dialogue | `NPCS` array |
| Shade whispers | `WHISPERS` array |
| Day length | `CYCLE` (seconds) |
| Dream-shift messages | `SHIFT_LINES` |
| Portal locations | `buildCrazy()` portal list |

## 🧰 Tech

- [Three.js r128](https://threejs.org/) (loaded from cdnjs)
- Vanilla JavaScript, HTML, CSS
- Web Pointer/Touch events for controls

## 📄 License

Vidhaan Mathur. See [LICENSE](LICENSE).
