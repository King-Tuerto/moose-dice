# Moose Dice — Claude Code Instructions

## Project
Browser-based dice game (Farkle/Moose Dice variant). Single self-contained HTML file.

## Architecture
- **Single file:** `index.html` — all HTML, CSS, JS inline. No build step, no dependencies.
- **No frameworks.** Vanilla JS only.

## Workflow
- Never work directly on main
- Feature branch: `feature/moose-dice-game`
- El Código builds, Nitpick reviews before any commit
- Paul approves PR before merge

## Game Rules (authoritative)
- 6 dice
- Scoring: 1=100, 5=50, three-of-a-kind = face×100 (three 1s = 1000)
- 4th matching die doubles 3OAK score; 5th doubles again
- 3 pairs = 1000
- Straight (1-2-3-4-5-6) = 1500
- Opening roll: 500 minimum to get on the board
- After opening: 350 minimum to bank
- Hot dice: all 6 dice score → roll all 6 again, points carry
- Bust: no keepers on roll → lose all turn points, advance turn
- Kept die can be picked back up (must leave ≥1 keeper set aside)
- First to 10,000 triggers final round — all others get one last turn to beat
- Flexible player count at game start

## File Structure
```
index.html   ← the entire game
CLAUDE.md    ← this file
```
