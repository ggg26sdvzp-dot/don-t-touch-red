# Don't Touch Red

A fast, neon-styled HTML arcade game where the player must keep a glowing orb alive by switching direction to avoid red obstacles.

## Overview

This project is built as a single-file browser game using HTML, CSS, and JavaScript. It features:

- a minimalist arcade presentation
- keyboard and touch/click controls
- procedural obstacle patterns and difficulty scaling
- power-ups such as shields, slow motion, score boosts, and dash
- local high-score tracking with `localStorage`
- optional sound effects when matching audio files are added

## How to run

Because this is a static HTML game, you can run it in any modern browser.

Option 1: open the file directly
- Open `dont-touch-red.html` in your browser.

Option 2: serve it locally
- From this folder, run:

```bash
python -m http.server 8000
```

- Then open:

```text
http://localhost:8000/dont-touch-red.html
```

## Controls

- Desktop: click or tap the game area to switch directions.
- Mobile: tap the canvas to flip the orb left/right.
- Goal: survive as long as possible while avoiding red walls.

## Game concept

The player is represented by a blue orb. Red blocks fall downward in patterns, and the orb must continuously shift from side to side to find safe gaps. The longer you survive, the faster and more chaotic the pattern becomes.

## Project structure

```text
.
├── dont-touch-red.html
├── README.md
└── sounds/                 (optional, add your own sound effects here)
```

## Optional sound files

The game already tries to load sound effects from a `sounds` folder. You can add these files if you want the full audio experience:

- `sounds/switch.mp3`
- `sounds/nearmiss.mp3`
- `sounds/combo.mp3`
- `sounds/death.mp3`
- `sounds/highscore.mp3`
- `sounds/powerup.mp3`
- `sounds/shield.mp3`

If a file is missing, the game simply skips it without breaking.

## Suggestions for this project

### 1. Add a proper start menu and settings screen
The game already has a basic menu, but it could be expanded with:

- difficulty selector
- sound/music toggle
- pause/resume button
- control sensitivity settings
- fullscreen option

### 2. Improve accessibility and polish
Consider adding:

- larger tap targets for mobile
- a more obvious pause state
- color-blind-friendly visuals
- stronger contrast for readability
- reduced-motion mode for users sensitive to animation

### 3. Add a leaderboard or save system
Right now the score is local only. You could add:

- player name entry
- persistent leaderboard with multiple scores
- daily/weekly challenge mode
- shareable score snapshots

### 4. Expand the game loop
This is a strong foundation for more gameplay variety, such as:

- boss waves
- special event modes
- more power-up types
- combo chains with richer rewards
- achievements or milestones

### 5. Improve asset design
The game already looks polished, but it could get even better with:

- custom sprite art instead of flat shapes
- animated background effects
- richer particle transitions
- more dramatic hit/death feedback
- themed visual skins or color palettes

### 6. Prepare for deployment
If you want to share the game publicly, consider:

- compressing assets
- testing on mobile browsers
- optimizing for low-end devices
- ensuring touch controls feel smooth on iPhone and Android
- hosting on GitHub Pages, Netlify, or Vercel

### 7. Add a mobile-first UX pass
Since the project is built for touch, a mobile-specific review is useful:

- ensure no accidental scrolling while playing
- improve button spacing
- consider vibration feedback (`navigator.vibrate`) on hits or score events
- tune obstacle density for smaller screens

## Possible next upgrades

A solid next step would be one of these:

1. Add a pause menu and difficulty settings.
2. Add sound/music assets and a richer audio layer.
3. Build a leaderboard and player profile system.
4. Add more enemy patterns and a boss wave mode.
5. Turn this into a mobile-optimized PWA.

## Notes

This project is a great example of a lightweight arcade game that is easy to run and easy to expand. The single-file structure makes it simple to prototype ideas quickly, while still leaving room for more advanced systems later.

## License

This project does not currently include a license file. If you plan to share or publish it publicly, it is a good idea to add one, such as MIT.
