# Neon Rift

A fast, top-down arcade space shooter in a retro neon vector style. Blast splitting asteroids, dodge hunter ships and survive escalating waves. The whole game is one self-contained `index.html` built with vanilla JavaScript and the Canvas API. There are no libraries and no image or sound assets, because every shape is drawn in code.

## Gameplay
- Pilot a ship with momentum-based movement and screen wrapping.
- Shoot asteroids, which split from large to medium to small.
- Hunter ships chase you across the screen.
- You have 3 lives and get 2 seconds of invulnerability after each hit.
- Clear each wave to start a harder one, with more enemies that move faster.
- Score points for each kill: small asteroids are worth the most, then ships, medium and large asteroids.
- Your final score and best score appear on the game-over screen.

## Controls
| Action | Input |
|---|---|
| Move | Arrow keys or WASD |
| Aim | Mouse |
| Fire | Space or left click (rate-limited) |
| Start / Restart | Enter, Space or click |

## Technical notes
- Single HTML file with inline CSS and JS.
- `requestAnimationFrame` game loop with a clamped delta time, so movement is frame-rate independent.
- Caps on bullets, asteroids, ships and particles keep performance smooth.
- Wave spawning uses a queue that releases enemies gradually.

## Run locally
Open `index.html` in any modern browser.

## Deploy
Import the repo into Vercel with the "Other" preset and no build command.
