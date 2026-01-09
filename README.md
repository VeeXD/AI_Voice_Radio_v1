# AI Voice Radio 🎙️

AI Voice Radio is an automated audio broadcast system built using n8n and OpenAI.  
It generates a continuous radio-style experience by summarizing live news, narrating stories, and converting everything into natural-sounding speech — all triggered with a single workflow execution.

---

## 🚀 What This Project Does

- Pulls live news from RSS feeds
- Summarizes news using an LLM
- Generates narrated stories (history, motivation, philosophy, real-world topics)
- Combines news and stories into a single radio-style script
- Converts the script into spoken audio using Text-to-Speech
- Runs end-to-end with no manual intervention once triggered

---

## 🧠 Why This Project

The goal of this project was to move beyond basic API calls and understand:
- AI workflow orchestration
- Event-driven automation using n8n
- Prompt engineering for time-based narration
- Combining multiple AI outputs into a single broadcast
- Cost-aware and deterministic AI execution

This project focuses on **system design**, not just model usage.

---

## 🧩 Architecture Overview

High-level workflow:

1. Schedule trigger initiates the workflow
2. RSS feeds provide live news data
3. LLM generates a summarized news script
4. LLM generates a narrated story
5. Both scripts are merged into a radio episode
6. Text-to-Speech generates spoken audio

> Audio playback and music integration are intentionally deferred to keep the core AI pipeline modular and extensible.

---

## 🛠 Tech Stack

- **n8n** – Workflow orchestration
- **OpenAI API** – LLM for text generation and TTS
- **RSS Feeds** – Live news ingestion
- **JSON-based workflow design**

---

## 📂 Repository Contents

- `workflow.json` – Exported n8n workflow (importable)
- `README.md` – Project documentation

---

## ▶️ How to Use

1. Import the workflow JSON into an n8n instance
2. Configure OpenAI credentials
3. Configure RSS feed sources
4. Execute the workflow manually or via schedule trigger
5. The workflow outputs a narrated audio file per execution

---

## 🔮 Planned Enhancements

- Automated local audio playback (macOS)
- Music integration (Spotify / YouTube Music)
- Voice rotation by day
- Topic-based content scheduling
- Cloud deployment

---

## 📌 Notes

- This repository focuses on AI orchestration and workflow design
- Music playback is intentionally excluded at this stage due to platform API constraints
- The system is designed to be extended without re-architecting the core workflow

---

## 👤 Author

Built by **Veekshith Sadam**  
AI, Data & Automation Enthusiast
