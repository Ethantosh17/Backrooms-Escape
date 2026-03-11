# Backrooms Escape

<img width="1249" height="735" alt="Screenshot 2026-03-11 at 6 40 47 AM" src="https://github.com/user-attachments/assets/54e5cf6b-5610-4921-a19f-037ca34793e1" />


A first-person browser
 horror game set in the Backrooms. Find the code. Reach the exit. Don't let it catch you!

## Play

Open `backrooms-escape.html` in any modern browser.

## Objective

1. Explore the maze and find the exit code on a note pinned to a wall somewhere in the level.
2. Once you have it, locate the exit door and escape.
3. Something is hunting you the entire time...

## Controls

| Input | Action |
|---|---|
| `W A S D` / Arrow Keys | Move |
| Mouse | Look |
| `ESC` | Pause / Resume |

## Features

- **Procedurally generated maze** — each run generates a unique 32×32 backrooms layout with rooms of varying sizes connected by winding two-cell-wide corridors, ensuring every room is reachable via a minimum spanning tree with added loops for disorientation.
- **Monster AI** — a wire-skeleton entity spawns in a distant room and actively hunts the player; it crouches as it closes in.
- **Atmospheric rendering** — Three.js 3D with exponential fog, fluorescent warm lighting, carpet/wall/ceiling textures, and vignette.
- **VHS overlay** — a full-screen post-process effect adds film grain, occasional tracking glitch bars, and a fake 1994 VHS timestamp that ticks in real time.
- **Procedural audio** — heartbeat, paper-rustle pickup sound, and win jingle all synthesized via the Web Audio API; no audio files required.
- **HUD** — live timer and code-found status indicator.

## Technical Details

- Single self-contained HTML file (~8 MB including embedded textures)
- Renderer: [Three.js r128](https://threejs.org/)
- No framework, no build toolchain

## Tips

- The note with the exit code appears on a random wall.
- Once you grab the code, the exit door turns green.
- Look out for the howler!
