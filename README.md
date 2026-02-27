# 📺 NEXUS NEWS — AI Broadcast System

> A fully browser-based, zero-cost AI news anchor with real-time lip sync, 3D avatar, and multilingual support. No backend. No server. Just one HTML file.

## 🎬 Demo

> 🌐 **Live Site:** https://bulletguitarist.github.io/AI-NEXUS-NEWS/

---

## ✨ Features

- ⚡ **Real-time AI script generation** via Groq API (500+ tokens/sec)
- 🎙️ **3D animated news anchor** rendered on HTML5 Canvas at 60fps
- 👄 **Live lip sync** — mouth moves in sync with every word spoken
- 🌍 **9 news topics** — World, Tech, Science, Finance, Space, Sports, Health, Film, Politics
- 🧾 **Multilingual** — English, Hindi, and Hinglish support
- 📱 **Fully responsive** — works on mobile, tablet, and desktop
- 💾 **Zero data collection** — API key stored only in your browser
- 🚀 **Deploy in 5 minutes** — single file, drag & drop to GitHub Pages or Netlify

---

## 🚀 Quick Start

### Step 1 — Get a Free Groq API Key
1. Go to **[console.groq.com](https://console.groq.com)**
2. Sign up with Google (free)
3. Click **API Keys** → **Create API Key**
4. Copy your key (starts with `gsk_...`)

> Free tier: **14,400 requests/day** — no credit card needed

### Step 2 — Deploy (Pick One)

#### Option A — GitHub Pages (The one which we used)
```
1. Fork or upload index.html to a new public repo
2. Go to Settings → Pages → Deploy from branch → main / (root)
3. Wait ~2 mins → your site is live at username.github.io/repo-name
```

#### Option B — Netlify
```
1. Go to netlify.com → Add new site → Deploy manually
2. Drag and drop index.html
3. Done — instant public URL
```

### Step 3 — Use It
1. Open your deployed URL
2. Paste your Groq API key → click **SAVE** → click **PING**
3. Choose a topic and language
4. Click **⚡ GENERATE**
5. Click **▶ BROADCAST** — watch the AI anchor come alive!

---

## 🛠️ Tech Stack

| Layer | Technology |
|-------|-----------|
| Language | Vanilla HTML / CSS / JavaScript (ES2022) |
| AI / LLM | Groq API — Llama 3.3 70B, Llama 3.1 8B, Mixtral 8x7B |
| Avatar Rendering | HTML5 Canvas 2D Context API |
| Text-to-Speech | Web Speech API (SpeechSynthesis) |
| Lip Sync | SpeechSynthesis `onboundary` events + vowel heuristics |
| Animation | `requestAnimationFrame` loop at 60fps |
| Fonts | Google Fonts (Orbitron, Space Mono, Rajdhani) |
| Hosting | GitHub Pages / Netlify (free static hosting) |
| Dependencies | **Zero** — no npm, no framework, no build step |

---

## 📁 Project Structure

```
nexus-news/
└── index.html        ← The entire application (single file, ~1400 lines)
```

That's it. One file.

---

## 🎛️ Configuration

All configuration is done in the browser UI:

| Setting | Options |
|---------|---------|
| AI Model | Llama 3.3 70B · Llama 3.1 8B ⚡ · Mixtral 8x7B · Gemma 2 9B |
| Topics | World · Tech · Science · Finance · Space · Sports · Health · Film · Politics |
| Language | 🇺🇸 English · 🇮🇳 Hindi · 🔀 Hinglish |
| Voice | All system voices available (browser-dependent) |
| Speed | 0.5x – 2.0x |
| Pitch | 0.1 – 2.0 |

---

## 🔒 Privacy & Security

- ✅ Your Groq API key is stored **only in your browser's localStorage**
- ✅ No analytics, no tracking, no cookies
- ✅ No server ever receives your data
- ✅ All API calls go directly from **your browser → Groq** over HTTPS
- ⚠️ Never share your API key publicly — rotate it at [console.groq.com](https://console.groq.com) if exposed

---

## 🐛 Troubleshooting

| Problem | Fix |
|---------|-----|
| PING fails with "Invalid key" | Generate a new key at console.groq.com |
| PING fails with "Network error" | You're probably testing locally (`file://`) — deploy to GitHub Pages first |
| No voice output | Try a different voice in the dropdown; Chrome on desktop works best |
| Page not found on GitHub Pages | Make sure the file is named exactly `index.html` (not `index (1).html`) |
| Blank page on GitHub Pages | Go to Settings → Pages and verify branch is set to `main` + `/(root)` |

---

## 🗺️ Roadmap

- [ ] Real news API integration (NewsAPI / GNews)
- [ ] WebGL 3D avatar upgrade
- [ ] ElevenLabs voice integration
- [ ] Video export (MediaRecorder API)
- [ ] Custom avatar photo upload
- [ ] Multi-anchor debate mode

## Author 
  THE BRATS
  (Ashvini Goswami & Jyotirmoy Mahapatra)
