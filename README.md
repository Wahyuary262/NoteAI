<div align="center">

# 🤖 NoteAI

### Smart Note Summarizer & AI Writing Assistant

[![Live Demo](https://img.shields.io/badge/demo-live-success?style=flat-square)](https://wahyuary262.github.io/NoteAI/)
[![License](https://img.shields.io/badge/license-MIT-blue?style=flat-square)](LICENSE)
[![MiMo API](https://img.shields.io/badge/powered%20by-Xiaomi%20MiMo-ff6b35?style=flat-square)](https://platform.xiaomimimo.com)
[![No Backend](https://img.shields.io/badge/backend-none-success?style=flat-square)]()
[![Single File](https://img.shields.io/badge/deploy-1%20HTML%20file-purple?style=flat-square)]()

**Browser-based AI writing assistant for students, professionals, and content creators.**

</div>

---

## 📖 Overview

**NoteAI** is a browser-based AI writing assistant that helps students, professionals, and content creators process long-form text using the **MiMo API**. Built as a single-page HTML app with real-time streaming output, session token tracking, and request history. Actively used for daily productivity tasks with consistent high-frequency API calls.

No backend. No build step. No dependencies. Just open the HTML file or deploy it anywhere.

---

## ✨ Features

| Mode | Use Case |
|------|----------|
| 📝 **Summarize** | Condense lectures, articles, meeting notes into key points |
| ✍️ **Rewrite** | Polish drafts to professional, clear, publication-ready text |
| 🔹 **Bullets** | Extract structured bullet points from messy notes |
| 🌐 **Translate** | Auto-detect & translate Indonesian ↔ English |
| ❓ **Q&A** | Generate 5 study questions + answers from any text |

**Plus:**
- ⚡ **Real-time SSE streaming** — output appears as the model generates it
- 📊 **Session tracking** — live token usage + request counter
- 💾 **Local-only API key** — stored in browser, never sent anywhere except MiMo
- 🎨 **Clean UI** — focused single-page design, zero distractions

---

## 👥 Who is this for?

- **🎓 Students** — summarize lectures, generate study Q&A, translate research papers
- **💼 Professionals** — rewrite emails, condense reports, extract action items from meetings
- **✍️ Content Creators** — repurpose long-form content into bullets, threads, translations
- **🌏 Bilingual users** — seamless ID ↔ EN workflows for daily writing

---

## 🚀 Quick Start

### 1. Get your MiMo API Key
- Register at [platform.xiaomimimo.com](https://platform.xiaomimimo.com)
- Go to **API Keys** → create a new key

### 2. Run the app

Single HTML file — pick your method:

```bash
# Option A — open directly in browser
open noteai.html         # macOS
xdg-open noteai.html     # Linux
start noteai.html        # Windows

# Option B — serve locally
npx serve .
# or
python -m http.server 8080
```

### 3. Use it
1. Paste your MiMo API key into the **API Key** field
2. Paste any text into the input area
3. Choose a mode (Summarize / Rewrite / Bullets / Translate / Q&A)
4. Hit **Run** — watch output stream in real-time

---

## 🌐 Deploy (Free)

### GitHub Pages (recommended)
```bash
# 1. Already on GitHub — just enable Pages
# Settings → Pages → Source: main branch → /(root) → Save
# 2. Live at: https://yourusername.github.io/NoteAI/
```

### Vercel
```bash
npm i -g vercel
vercel --prod
```

### Cloudflare Pages
- Connect repo at [pages.cloudflare.com](https://pages.cloudflare.com)
- Build command: *(none)*
- Output directory: `/`

### Netlify
- Drag & drop the folder to [app.netlify.com/drop](https://app.netlify.com/drop)

---

## 🔧 Tech Stack

```yaml
Frontend:    Vanilla HTML + CSS + JavaScript (zero dependencies)
AI Backend:  Xiaomi MiMo API (api.xiaomimimo.com/v1)
Streaming:   Server-Sent Events (SSE) for real-time output
Storage:     localStorage (API key, history — local only)
Build:       None — pure static HTML
```

---

## 📁 Project Structure

```
NoteAI/
├── noteai.html     # entire app — one file, ~20KB
└── README.md       # this file
```

---

## 🤖 Supported Models

| Model | Best For |
|-------|----------|
| `MiMo-7B-RL` | Fast, lightweight — daily tasks, summaries, translations |
| `MiMo-72B-RL` | Heavy lifting — complex rewriting, nuanced Q&A |

---

## 📊 Usage Tracking

The top bar shows **session token usage** + **request count** in real-time so you can monitor API consumption without leaving the app.

---

## 🔒 Privacy & Security

- ✅ API key stored **locally in your browser only** (`localStorage`)
- ✅ No data sent to any server **other than MiMo API**
- ✅ No analytics, no tracking, no ads, no telemetry
- ✅ No cookies, no third-party scripts
- ✅ Works fully offline once loaded (except for AI calls)

---

## 💡 Use Cases

- 📚 Summarize a 30-page PDF before an exam
- 📧 Rewrite a casual email into a professional one
- 📝 Convert meeting transcripts into action-item bullets
- 🌐 Translate Indonesian research papers into English drafts
- ❓ Auto-generate quiz questions from study material
- 🐦 Repurpose blog posts into Twitter threads (via bullets)
- 📰 Daily news digest condensation

---

## 🎯 Roadmap

- [ ] Custom system prompts per mode
- [ ] Export results (Markdown / PDF / DOCX)
- [ ] Request history persistence (IndexedDB)
- [ ] Dark mode toggle
- [ ] More language pairs (JP, ZH, KR)
- [ ] Image input (OCR → process)

---

## 🤝 Contributing

PRs welcome. This is a single-file app by design — keep it that way unless there's a strong reason.

```bash
git clone https://github.com/Wahyuary262/NoteAI.git
cd NoteAI
# edit noteai.html
# open in browser to test
git commit -am "feat: ..."
git push
```

---

## 📄 License

MIT — free to use, modify, deploy, monetize.

---

<div align="center">

Built for the **Xiaomi MiMo Orbit 100T Token Creator Program** 🚀

**Daily-driver AI writing tool. No bloat. No backend. Just results.**

</div>
