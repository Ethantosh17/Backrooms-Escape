# Backrooms Escape

# <img width="1249" height="735" alt="Screenshot 2026-03-11 at 6 40 47 AM" src="https://github.com/user-attachments/assets/54e5cf6b-5610-4921-a19f-037ca34793e1" />

A first-person browser horror game set in the Backrooms. Find all four code digits, enter them at the exit keypad, and escape — before it catches you.

## Play

Open `backrooms-escape.html` in any modern browser.

## Objective

1. Explore the maze and find **4 notes** pinned to walls across Level 0, each showing one digit of a 4-digit code.
2. Memorize the digits in order.
3. Locate the **exit door** and interact with the **keypad** beside it.
4. Enter the correct code to escape.

Something is hunting you the entire time.

## Controls

| Input | Action |
|---|---|
| `W A S D` / Arrow Keys | Move |
| `Shift` | Sprint |
| `Space` | Jump |
| `Mouse` | Look |
| `E` | Interact with keypad / close keypad |
| `ESC` | Pause |
| Click overlay | Resume |

## Features

- **Procedurally generated maze** — each run generates a unique 32×32 backrooms layout with rooms of varying sizes connected by winding two-cell-wide corridors, ensuring every room is reachable via a minimum spanning tree with added loops for disorientation.
- **4-digit code system** — four separate notes are scattered across the level, each bearing one digit labeled by position. Memorize them and enter the code at the 3D keypad beside the exit door.
- **A\* pathfinding monster** — a wire-skeleton entity navigates the maze using A\* pathfinding, actively hunting the player around corners. It wanders when out of range and chases when it spots you, growing faster over time.
- **Cannon.js physics** — full rigid-body physics for the player and monster, with static collision bodies generated from the procedural map at runtime.
- **Atmospheric rendering** — Three.js 3D with exponential fog, fluorescent warm lighting, carpet/wall/ceiling textures, and vignette.
- **VHS overlay** — a full-screen post-process effect adds film grain, occasional tracking glitch bars, and a fake 1994 VHS timestamp that ticks in real time.
- **Procedural audio** — heartbeat, paper-rustle, and win jingle all synthesized via the Web Audio API; no audio files required. Audio suspends on pause.
- **HUD** — live timer and status indicator.

## Technical Details

- Single self-contained HTML file (~8 MB including embedded textures)
- Renderer: [Three.js r128](https://threejs.org/)
- Physics: [Cannon.js 0.6.2](https://github.com/schteppe/cannon.js)
- No framework, no build toolchain

## Tips

- Each note is labeled **DIGIT X / 4** — note the order carefully.
- Walk up to the keypad beside the door and press **E** to open it.
- Sprint to pull away from the monster — but it gets faster the longer you survive.
- Look out for the howler!
