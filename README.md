# Tonewave - A Python Desktop Music Player

> A personal desktop music player built with **CustomTkinter** and **Pygame Mixer**.  
> Clean dark UI, album art display, full playlist control, and smooth playback — all in one Python file.

---

## 🎵 What is Tonewave?

Tonewave is a lightweight desktop music player that lets you load, organize, and play your local MP3 and WAV files with a polished dark-themed interface. It features real-time progress tracking, album art extraction, loop modes, shuffle, and volume control — built entirely in Python.

---

## ✨ Features

- ✅ Load and play **MP3 and WAV** files
- ✅ **Playlist management** — add, scroll, and clear tracks
- ✅ **Album art extraction** — displays embedded cover art from MP3 metadata
- ✅ **Progress bar** with seek support — click to jump to any position
- ✅ **Play / Pause / Stop / Previous / Next** controls
- ✅ **Shuffle** — randomly jumps to a different track
- ✅ **Loop modes** — Loop Off, Loop All, Loop One
- ✅ **Volume slider** with live adjustment
- ✅ Real-time **track timer** display (`current / total`)
- ✅ Dark-themed UI using **CustomTkinter**
- ✅ Gracefully handles missing assets and audio devices

---

## 🛠️ Requirements

Install dependencies with:

```bash
pip install customtkinter pygame mutagen Pillow
```

---

## 🔑 Setup

1. Clone or download this repository
2. Make sure your `assets/` and `Gray/` folders are present (see [Project Structure](#-project-structure) below)
3. Run the player:

```bash
python Tonewave.py
```

---

## 📁 Project Structure

```
tonewave_music_player/
├── Tonewave.py               # Main application
├── assets/
│   └── Icon/
│       └── music-app.ico     # Window icon
└── Gray/                     # UI button images
    ├── play-button.png
    ├── pause-button.png
    ├── next-button.png
    ├── previous-button.png
    ├── shuffle-button.png
    ├── loop-off-button.png
    ├── loop-all-button.png
    ├── loop-one-button.png
    ├── speaker-button.png
    ├── add-button.png
    ├── clear-button.png
    └── no-album.png          # Fallback when no album art is found
```

---

## 🖼️ Assets

Tonewave uses image-based buttons loaded from the `Gray/` folder. These are standard PNG icons for playback controls. If any asset is missing, the app will attempt to locate it automatically using a recursive file search before falling back gracefully.

---

## 🎮 How to Use

| Action | How |
|---|---|
| Add tracks | Click the **+** button in the playlist panel |
| Play a track | Click any track in the playlist |
| Play / Pause | Click the center play button |
| Seek | Drag or click the progress bar |
| Next / Previous | Use the arrow buttons |
| Shuffle | Click the shuffle button |
| Loop | Click the loop button to cycle through Off → All → One |
| Volume | Drag the volume slider |
| Clear playlist | Click the **X** button in the playlist panel |

---

## 📦 Dependencies

| Library | Purpose |
|---|---|
| `customtkinter` | Dark-themed modern UI framework |
| `pygame.mixer` | Audio playback engine |
| `mutagen` | MP3 metadata & album art extraction |
| `Pillow` | Image processing for album art display |
| `tkinter` | File dialog (built into Python) |

---

## ⚠️ Disclaimer

This project was created for educational purposes as part of a school activity. Built to practice Python GUI development, audio handling, and file management. No commercial intent whatsoever.

---

*"Your music. Your wave." — ReCreatem3*
