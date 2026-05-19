# NoteAI — Smart Note Summarizer

> AI-powered writing assistant built with plain HTML + JS, powered by Xiaomi MiMo API.

---

## ✨ Features

| Mode | Description |
|---|---|
| **Summarize** | Condenses long text into a concise paragraph |
| **Rewrite** | Improves clarity and professionalism of writing |
| **Bullets** | Converts text into structured bullet points |
| **Translate** | Auto-detects and translates between Indonesian ↔ English |
| **Q&A** | Generates 5 questions and answers from the text |

---

## 🚀 Quick Start

### 1. Get your MiMo API Key
- Register at [platform.xiaomimimo.com](https://platform.xiaomimimo.com)
- Go to **API Keys** section and create a new key

### 2. Run the app
Since this is a single HTML file, no installation needed:

```bash
# Option A — just open directly
open noteai.html

# Option B — serve locally
npx serve .
# or
python -m http.server 8080
```

### 3. Use it
1. Paste your MiMo API key into the **API Key** field
2. Paste any text into the input area
3. Choose a mode (Summarize / Rewrite / Bullets / Translate / Q&A)
4. Click **Run**

---

## 🌐 Deploy (Free)

### Vercel
```bash
npm i -g vercel
vercel
```

### GitHub Pages
1. Push this repo to GitHub
2. Go to **Settings → Pages**
3. Set source to `main` branch → Save
4. Your app is live at `https://yourusername.github.io/noteai`

---

## 🔧 Tech Stack

- **Frontend:** Vanilla HTML, CSS, JavaScript (zero dependencies)
- **AI Backend:** Xiaomi MiMo API (`api.xiaomimimo.com/v1`)
- **Streaming:** Server-Sent Events (SSE) for real-time output
- **Storage:** API key saved to `localStorage` (local only, never sent anywhere else)

---

## 📁 Project Structure

```
noteai/
├── noteai.html     # entire app — one file
└── README.md       # this file
```

---

## 🤖 Supported Models

| Model | Notes |
|---|---|
| `MiMo-7B-RL` | Faster, lighter — good for most tasks |
| `MiMo-72B-RL` | More powerful — better for complex rewriting |

---

## 📊 Usage Tracking

The app tracks **session token usage** and **request count** in the top bar so you can monitor your API consumption in real time.

---

## 🔒 Privacy

- Your API key is stored **locally in your browser only**
- No data is sent to any server other than the MiMo API
- No analytics, no tracking, no ads

---

## 📄 License

MIT — free to use, modify, and deploy.

---

Built for the **Xiaomi MiMo Orbit 100T Token Creator Program** 🚀
