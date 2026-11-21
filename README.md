# 🎓 Campus Clash

**A free, browser-based college fighting game — 11 fighters, 8 arenas, zero downloads.**
*Attendance kam, attitude full.* 🥊

[![Play Now](https://img.shields.io/badge/▶_Play_Now-campusclash--lime.vercel.app-brightgreen?style=for-the-badge)](https://campusclash-lime.vercel.app/)
[![Version](https://img.shields.io/badge/version-v26-blue?style=for-the-badge)](https://github.com/kirtivardhansingh29/Campus-Clash/releases)
[![Tech](https://img.shields.io/badge/built_with-Three.js_%2B_WebAudio_%2B_WebRTC-orange?style=for-the-badge)](https://threejs.org/)

Campus Clash is a light-hearted, slapstick fighting game set in a fictional Indian college. Pick your fighter — the topper, the backbencher, the hostel warden, the canteen bhaiya, even the placement cell boss — choose an arena, and settle campus scores the funny way. No gore, only gags.

---

## 🎮 Play the Game

| | |
|---|---|
| **▶ Play online (recommended)** | **https://campusclash-lime.vercel.app/** |
| Mirror link | https://muse.ai/s/campus-clash-xdn6vpwmxjxvkxz/ploNDeK3c5Nxuvn8JenoXoGWJ_wmN2w7_5gqVee1kmc |
| 📸 Instagram | [@campusclashofficial](https://www.instagram.com/campusclashofficial/) |

No install, no sign-up. Works on desktop and mobile (touch controls included).

## ✨ Features

- **11 playable fighters + 1 boss**, each with unique poses, a signature move, a style move and a 3-beat cinematic super (flat 30% HP — balance by presentation, not power tiers)
- **Attendance Meter** — the super meter is the attendance register; fill it to unlock your special, and tied rounds are decided by attendance, exactly like real college
- **8 arenas** — Canteen, Library, Hostel, Auditorium, Classroom, Main Gate, Lab and the Placement Cell Office, each with its own crowd, news ticker and music flavour
- **Spoken punchlines** — every fighter actually *says* their catchphrase on Special and Style moves, on top of a fully procedural synth soundtrack
- **Online multiplayer** — create a room, share the code, fight a friend from another device (peer-to-peer WebRTC, host-authoritative, automatic reconnect)
- **Marksheet result card** — every match ends with a shareable marksheet, PASS/BACK stamps included
- **Performance-tuned** — ~9 MB total, adaptive quality scaling, touch fight-pad with multi-touch support

## 🥋 The Roster

| Fighter | Archetype | Super Move |
|---|---|---|
| **Adarsh** | The Ideal Loser | Deploy Kar Diya! |
| **Topper** | The Rank Machine | Notes Tornado |
| **Backbencher** | The Last-Bench Legend | Proxy Punch |
| **Warden Sir** | The 10 Baje Wala | Gate Band 10 Baje! |
| **Canteen Bhaiya** | The Maggi Master | Maggi Missile |
| **Lab Madam** | The Internal-Marks Empress | 6 Se 9! |
| **AI Dog** | Made in Greater Noida | Viral Bark Blast |
| **CR** | The Notice Machine | Notice Forward Blast |
| **Vidya** | The Daily-Attending Topper | Main Jaungi, Meri Marzi Hai! |
| **Eventwala** | The Clubs Hype Man | Sab Event Mein Aao! |
| **Placement Cell Sir** *(boss)* | The Final Hurdle | CTC Mirage |

## 🕹️ Game Modes

- **VS CPU** — quick fight against the computer (3 difficulties)
- **2 Player** — same-keyboard versus, hostel-style
- **Semester Mode** — an 8-stage campaign ladder ending at the Placement Cell boss, who fights by a different rule (Shortlist Meter)
- **Orientation Day** — practice mode
- **Online** — room-code multiplayer over the internet

## ⌨️ Controls

**Player 1:** `A`/`D` move · `W` jump · `S` crouch · hold away to block (and walk back) · `J` punch · `K` kick · `L` grab · `U` style move · `SPACE` special

**Player 2:** Arrow keys move · `,` punch · `.` kick · `/` grab · `M` style move · `Right Shift` special

**Mobile:** on-screen fight-pad (directions, punch/kick/grab/style + special) with multi-touch — signatures like ▼+KICK work on touch too.

Rounds are 60 seconds, best of 3.

## 🛠️ Tech Stack

| Layer | Technology |
|---|---|
| Rendering | Three.js — 3D arenas with 2.5D photo-cutout fighters |
| Game logic | Vanilla JavaScript, fixed-timestep simulation (60 fps), fully documented frame data |
| Audio | Procedural WebAudio synth (music, SFX, crowd) + recorded voice clips in `assets/voice/` |
| Multiplayer | WebRTC via PeerJS — room codes, TURN relay fallback, heartbeat watchdog + reconnect grace |
| Persistence | `localStorage` (progress, settings, unlocks) |
| Hosting | Vercel (static) |

## 📁 Project Structure

```
Campus-Clash/
├── index.html        # The entire game — a single self-contained file
├── assets/
│   └── voice/        # Fighter punchline clips (MP3)
├── robots.txt
├── sitemap.xml
└── README.md
```

## 🚀 Run Locally

```bash
git clone https://github.com/kirtivardhansingh29/Campus-Clash.git
cd Campus-Clash
npx serve .        # or: python -m http.server
```

Open the local URL in any modern browser. (A static server is recommended — the voice clips are fetched from `assets/voice/` at runtime.)

## 🗺️ Roadmap

- [x] Core fighting system with documented frame data & balance model
- [x] Semester Mode campaign + boss rule-twist
- [x] Online room-code multiplayer with reconnect handling
- [x] Mobile touch controls & performance passes
- [x] Fighter voice lines
- [ ] Cartoon-SFX layered audio mix
- [ ] Fight start/end announcer calls
- [ ] Google Search Console indexing

## ⚠️ Disclaimer

Campus Clash is a work of fiction. The college, characters and events are imaginary and made purely for fun — any resemblance to your own campus life is purely coincidental (and probably accurate). 😉

## 👨‍💻 Author

**Kirti Vardhan Singh** — B.Tech IT (2024–28), Greater Noida, India
[GitHub](https://github.com/kirtivardhansingh29) · [LinkedIn](https://www.linkedin.com/in/kirtivardhansingh67)

---

*Made with ❤️ and very low attendance.*
