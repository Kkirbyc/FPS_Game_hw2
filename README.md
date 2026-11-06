# HW2 — First Person Blueprint Game

Unreal Engine **5.0.3**. Editable coursework project based on the First Person template with Starter Content.

## Submission links

- Project: https://github.com/Kkirbyc/FPS_Game_hw2
- Demonstration video: **Pending recording and upload.**

## Open and play

1. Download the repository ZIP and extract it, or clone this repository.
2. Open `HW2_FPS.uproject` in Unreal Engine 5.0.3. Allow shaders to compile.
3. The Menu map opens by default. Use Play, then START GAME.
4. Use Standalone Game to test the QUIT button closing the game window.

The repository includes the editable `.uproject`, `Content`, and `Config`. A packaged executable is not included. Editor caches regenerate locally. The project uses the engine's PythonScriptPlugin and EditorScriptingUtilities editor plugins; no external plugin is required.

## Controls

| Input | Action |
| --- | --- |
| WASD | Move |
| Mouse | Look |
| Left mouse button | Fire after collecting the rifle |
| Space | Jump |
| Mouse on menu | START GAME / QUIT |

## Gameplay and demonstration checklist

- Map sequence: **Menu → Arena01 → Arena02 → Menu**. Arena01 has a rectangular layout with central cover; Arena02 has an L-shaped layout.
- Each gameplay map contains 3 targets, 3 hazards, 2 ammunition pickups, and 2 health pickups.
- Targets have 100 health and receive 25 damage per projectile hit: four hits destroy a target. Walking into a target is not a projectile hit.
- Starting ammunition is 12. Each shot consumes one round. At zero ammunition, firing is blocked. An ammunition pickup adds 12 rounds and disappears.
- Player health starts at 100. Entering a hazard removes 25 health; leaving and re-entering causes another hit. A health pickup adds 50, capped at 100, and disappears.
- On death, the current gameplay map reloads, resetting the player and targets.
- HUD shows ammunition, health, and destroyed targets / total targets.
- Destroying all targets automatically advances to the next map; clearing Arena02 returns to Menu. Starting again resets the game state.

## Verification status

The author manually tested the gameplay in the editor, including target damage, ammunition depletion and pickups, health damage and pickups, map progression, restarting from the menu, and death/reload in both maps. The QUIT button was tested in Standalone Game. These are manual test results, not automated verification.

The Game Default Map is Menu, and the packaging map list includes Menu, Arena01, and Arena02. A packaged Windows build has not been produced or tested. The demonstration video and final timestamps will be added after recording.
