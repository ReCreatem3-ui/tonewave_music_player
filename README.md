# Tonewave - A Python Desktop Music Player
> A personal desktop music player built with **CustomTkinter** and **Pygame Mixer**.  
> Clean dark UI, album art display, full playlist control, and smooth playback — all in one Python file.

---

## What is Tonewave?

Tonewave is a lightweight desktop music player that lets you load, organize, and play your local MP3 and WAV files with a polished dark-themed interface. It features real-time progress tracking, album art extraction, loop modes, shuffle, and volume control — built entirely in Python.

---

## Features

- Load and play **MP3 and WAV** files
- **Playlist management** — add, scroll, and clear tracks
- **Album art extraction** — displays embedded cover art from MP3 metadata
- **Progress bar** with seek support — click to jump to any position
- **Play / Pause / Previous / Next** controls
- **Shuffle** — randomly jumps to a different track
- **Loop modes** — Loop Off, Loop All, Loop One
- **Volume slider** with mute toggle and live adjustment
- Real-time **track timer** display (`current / total`)
- Dark-themed UI using **CustomTkinter**
- Minimum window size locked at **800x650**
- Keyboard shortcuts: `Space`, `Arrow keys`
- Gracefully handles missing assets using recursive file search

---

## Requirements

Install dependencies with:

```bash
pip install customtkinter pygame mutagen Pillow
```

---

## Setup

1. Clone or download this repository
2. Make sure your `assets/` folder is present (see [Project Structure](#project-structure) below)
3. Run the player:

```bash
python tonewave_music_player.py
```

---

## Project Structure

```
tonewave_music_player/
├── tonewave_music_player.py        # Main application
└── assets/
    ├── icon/
    │   └── music_app.ico           # Window and taskbar icon
    └── buttons/
        └── gray_buttons/           # UI button images
            ├── play_button.png
            ├── pause_button.png
            ├── next_button.png
            ├── previous_button.png
            ├── shuffle_button.png
            ├── loop_off_button.png
            ├── loop_all_button.png
            ├── loop_one_button.png
            ├── speaker_button.png
            ├── speaker_button_mute.png
            ├── add_button.png
            ├── clear_button.png
            └── no_album.png        # Fallback when no album art is found
```

---

## Assets

Tonewave uses image-based buttons loaded from the `assets/buttons/gray_buttons/` folder. These are standard PNG icons for playback controls. If any asset is missing, the app will attempt to locate it automatically using a recursive file search across multiple base paths before falling back gracefully.

---

## How to Use

<img width="2560" height="1440" alt="Tonewave User Manual" src="https://github.com/user-attachments/assets/e4d169e6-9cf7-4624-a5b2-05b7d93e0456" />

| Action | How |
|---|---|
| Add tracks | Click the **+** button in the playlist panel |
| Play a track | Click any track in the playlist |
| Play / Pause | Click the center play button or press `Space` |
| Seek | Drag or click the progress bar |
| Next / Previous | Use the arrow buttons or press `Right` / `Left` |
| Shuffle | Click the shuffle button |
| Loop | Click the loop button to cycle through Off -> All -> One |
| Volume | Drag the volume slider or press `Up` / `Down` |
| Mute | Click the speaker icon |
| Clear playlist | Click the trash button in the playlist panel |

---

## Keyboard Shortcuts

| Key | Action |
|---|---|
| `Space` | Play / Pause |
| `Right Arrow` | Next track |
| `Left Arrow` | Previous track |
| `Up Arrow` | Volume up |
| `Down Arrow` | Volume down |

---

## Dependencies

| Library | Purpose |
|---|---|
| `customtkinter` | Dark-themed modern UI framework |
| `pygame.mixer` | Audio playback engine |
| `mutagen` | MP3 metadata and album art extraction |
| `Pillow` | Image processing for album art display |
| `tkinter` | File dialog (built into Python) |
