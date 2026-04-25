# 📧 AI Email Responder – Gmail Add-on

> A smart Gmail add-on powered by Google Gemini API that generates context-aware, customizable email drafts directly inside Gmail.

![Google Apps Script](https://img.shields.io/badge/Google_Apps_Script-4285F4?style=flat-square&logo=google&logoColor=white)
![Gemini API](https://img.shields.io/badge/Gemini_API-8E24AA?style=flat-square&logo=google&logoColor=white)
![Gmail](https://img.shields.io/badge/Gmail_Add--on-EA4335?style=flat-square&logo=gmail&logoColor=white)

---

## 📌 Project Overview

The AI Email Responder integrates Generative AI directly into Gmail — allowing users to generate complete, professional email drafts with a single click. Users retain full control over tone, length, and style before sending.

**No external tools. No tab-switching. Draft replies right inside Gmail.**

---

## ✨ Features

- **Context-aware drafting** — analyzes email content and generates relevant replies
- **Customizable output** — choose tone (professional / friendly / persuasive), length, style, language
- **Inline sidebar UI** — works inside Gmail, no separate app needed
- **Full user control** — edit, regenerate, preview, save as draft, or send directly
- **Emoji toggle** — optionally include emojis in the response

---

## 🏗️ Architecture

```
Gmail Sidebar (Add-on UI)
        ↓
Google Apps Script (Backend)
        ↓
Gemini API (LLM — generates draft)
        ↓
Response displayed back in Gmail sidebar
```

---

## 🗂️ Project Structure

```
ai-email-responder/
│
├── Code.gs                        # Main Apps Script backend
├── Sidebar.html                   # Gmail sidebar UI (HTML/CSS/JS)
├── appsscript.json                # Add-on manifest & scopes
└── README.md
```

---

## 🚀 How to Deploy

1. Go to [Google Apps Script](https://script.google.com) and create a new project
2. Copy `Code.gs` and `Sidebar.html` into the editor
3. Update `appsscript.json` with your Gemini API key scope
4. Click **Deploy → New Deployment → Gmail Add-on**
5. Open Gmail — the add-on appears in the right sidebar

---

## 🎛️ User Options

| Setting | Options |
|---|---|
| Tone | Professional · Friendly · Persuasive |
| Length | Short · Medium · Detailed |
| Style | Formal · Casual · Polished |
| Language | English + others |
| Emojis | On / Off |

---

## 🔑 API Setup

Add your Gemini API key in `Code.gs`:
```javascript
const GEMINI_API_KEY = 'YOUR_API_KEY_HERE';
```

---

*Built by [Krisha Shah](https://www.linkedin.com/in/krishas7) · Mumbai, India*
