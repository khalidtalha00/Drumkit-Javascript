# Drum 🥁 Kit

A simple browser-based drum kit built with vanilla HTML, CSS, and JavaScript. Play drum sounds either by clicking the on-screen buttons or by pressing the corresponding keys on your keyboard.

## Features

- 7 drum pads: tom1, tom2, tom3, tom4, snare, crash, and kick
- Click-to-play and keyboard-to-play support
- Clean, styled UI with custom drum pad icons

## Key Mapping

| Key | Sound  |
|-----|--------|
| W   | Tom 1  |
| A   | Tom 2  |
| S   | Tom 3  |
| D   | Tom 4  |
| J   | Snare  |
| K   | Crash  |
| L   | Kick   |

## Project Structure

```
.
├── index.html       # Markup for the drum kit UI
├── styles.css        # Styling for buttons, layout, and background
├── index.js          # Sound playback logic (click + keypress)
├── images/            # Drum pad icons (tom1.png, tom2.png, etc.)
└── sounds/            # Drum sound audio files (.mp3)
```

> **Note:** The `images/` and `sounds/` folders referenced in the CSS and JS must exist alongside these files with the appropriate assets for the kit to display and play correctly.

## Getting Started

1. Clone or download this repository.
2. Make sure the `images/` and `sounds/` folders are present with the required assets.
3. Open `index.html` in your browser — no build step or server required.

## How It Works

- `index.js` listens for both `click` events on the drum buttons and `keypress` events on the document.
- The `playSound` function uses a `switch` statement to match the pressed key (or clicked button's label) to the corresponding `Audio` object and plays it.
- `styles.css` handles the visual styling, including background images for each drum pad and a `.pressed` class for visual feedback (if wired up to be toggled on press).

## Credits

Made by Talha Khalid.