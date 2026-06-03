# 🎂 For Heena — Happy Birthday

A luxurious, interactive birthday tribute page built with pure HTML, CSS, and JavaScript. Designed as a heartfelt gift featuring an immersive music player, animated memory cards, a virtual birthday cake, and more — all wrapped in a soft glassmorphism aesthetic.

🌐 **[View Live →](https://thvariableyt.github.io/birthday/)**

---

## ✨ Features

- **🎁 Intro Screen** — An elegant gift-box splash screen with a glowing animation to "begin the celebration"
- **🎂 Birthday Cake** — An interactive hazelnut truffle cake with flickering candles; swipe or tap to blow them out and reveal a heartfelt wish message
- **🃏 Memories Archipelago** — Parallax-scrolling 3D flip cards, each revealing a personal memory on the back
- **🎵 Cosmic Sync Music Player** — A vinyl-record-style player with:
  - Pre-loaded tracks (*Your Thoughts*, *Saajna*, *Perfect*)
  - Live synced lyrics via `.lrc` files
  - Adjustable lyric font size
  - Upload your own audio + lyrics (`.lrc` / `.txt`)
- **🫙 Vial of Luminescence** — A glowing potion bottle that reveals a randomised appreciation note on every tap
- **🎼 Harp of Whispers** — A playable musical harp with 6 chime bars (C D E G A C); swipe or tap to play celestial tones
- **🌟 Sparkle Canvas** — Cursor-following gold sparkle particles rendered on a full-screen canvas overlay
- **🎶 Ambient Mood Music** — A toggleable soft ambient pad soundtrack generated with the Web Audio API

---

## 🗂️ File Structure

```
birthday/
├── index.html          # Main page — all UI, styles & scripts
├── Perfect.m4a         # Audio track: Perfect
├── Perfect.lrc         # Synced lyrics for Perfect
├── Saajna.flac         # Audio track: Saajna
├── Saajna.lrc          # Synced lyrics for Saajna
├── Your Thoughts.flac  # Audio track: Your Thoughts
├── Your Thoughts.lrc   # Synced lyrics for Your Thoughts
└── .gitattributes      # Git config (LFS / line endings)
```

---

## 🛠️ Tech Stack

| Technology | Usage |
|---|---|
| HTML5 / CSS3 | Page structure & custom animations |
| [Tailwind CSS](https://tailwindcss.com/) (CDN) | Utility-first styling |
| [GSAP + ScrollTrigger](https://greensock.com/gsap/) | Parallax scroll & card flip animations |
| [Font Awesome 6](https://fontawesome.com/) | Icons |
| [Google Fonts](https://fonts.google.com/) | *Playfair Display* & *Plus Jakarta Sans* |
| Web Audio API | Harp chimes, ambient pads & procedural music |

---

## 🚀 Running Locally

Because the audio files are loaded via relative paths, you need a local server to avoid browser CORS restrictions.

**Option 1 — VS Code Live Server**
1. Open the project folder in VS Code
2. Right-click `index.html` → **Open with Live Server**

**Option 2 — Python**
```bash
python -m http.server 8000
# Then open http://localhost:8000
```

**Option 3 — Node.js**
```bash
npx serve .
```

> ⚠️ Opening `index.html` directly via `file://` will cause audio playback to fail.

---

## 🎵 Adding Custom Tracks

1. Click **"+ Add Your Own Song"** at the bottom of the music player
2. Enter the song name
3. Upload an audio file (MP3, FLAC, M4A, etc.)
4. Optionally upload a `.lrc` lyrics file for live lyric sync
5. Click **Add Song** — it appears instantly in the playlist!

---

## 📄 License

This project is a personal gift and is not intended for redistribution. All audio tracks belong to their respective rights holders.

---

<p align="center">Made with 💛 by <a href="https://github.com/ThVariableYT">ThVariableYT</a> — exclusively for Heena</p>
