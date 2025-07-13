# 🛡️ Scam Defender Bot

A Telegram-based bot that helps users detect, understand, and report online scams in real-time.  
Built using [n8n](https://n8n.io) and **Gemini 2.5 Flash API**, this smart assistant accepts voice, text, documents, and images — and guides users with alerts, risk ratings, and reporting help.

---

## 🔍 Features

- 🧠 **Gemini 2.5 Flash API** detects scams from:
  - Text
  - Voice messages
  - PDFs / Documents
  - Screenshots / Images
- 🗣 **Voice message support** using Gemini's direct audio input
- 📊 **Google Sheets Logging** (only if scam risk is medium 🔶 or high 🔴)
  - Stores: user input, Gemini response, scam risk level, timestamp, Telegram user ID
- 📂 **PDF/Document Uploads** handled via Gemini (not RAG)
- 🔔 **Latest Scam Alerts**: type `latest`, `scams`, or `alerts` to get recent scams
- 📝 **Complaint Guidance**: type `report` or `complaint` to know where and how to report

---

## 🛠️ Tech Stack

- [n8n](https://n8n.io) – Workflow automation
- [Gemini 2.5 Flash](https://ai.google.dev/gemini-api/docs) – Multimodal LLM
- [Google Sheets API](https://developers.google.com/sheets/api) – Log suspicious cases
- [Telegram Bot API](https://core.telegram.org/bots/api)

---
🔒 Note: API keys and tokens are excluded for security. Replace placeholders with your own to test the workflow.
---

## 🖼️ Demo

📎 [View the bot demo (PDF)](scam bot.pdf)

---

## 📂 Repository Contents

| File / Folder                      | Description                                 |
|-----------------------------------|---------------------------------------------|
| `scam-defender-bot-workflow.json` | Exported n8n bot logic                      |
| `scam bot.pdf`                    | Screenshots of bot in action                |
| `README.md`                       | This file                                   |

---

## 🚀 How It Works

1. Users send **text**, **voice**, **PDFs**, or **images** to the Telegram bot.
2. Gemini 2.5 Flash analyzes the content and detects potential scams.
3. If the **risk is medium/high**, the interaction is saved to Google Sheets.
4. Bot shows risk levels:
   - 🟢 Safe
   - 🟡 Caution
   - 🔴 Danger
5. Bot provides links for:
   - Latest scam alerts (`alerts`, `latest`)
   - Where to report scams (`report`, `complaint`)

---

## 🧪 How to Use Locally

1. Import `scam-defender-bot-workflow.json` in your **n8n** instance
2. Set up credentials:
   - Telegram Bot Token
   - Google Sheets
   - Gemini 2.5 API key (from [Gemini API Docs](https://ai.google.dev/gemini-api/docs))
3. Deploy & start interacting with the Telegram bot

---

## ✍️ Author

**Haindavi Sira**  
🎓 B.Tech CSE (AI & ML) | VNRVJIET  
🧠 AI enthusiast • Automation builder  
🌐 [LinkedIn](https://www.linkedin.com/in/haindavi-sira-b0350028b?utm_source=share&utm_campaign=share_via&utm_content=profile&utm_medium=android_app)

---

## ⭐ Support

Found this useful? ⭐ Star the repo and share feedback!

