# Speech Transcribe & Summarize

Python FastAPI pipeline that turns meeting audio into a transcript plus structured summary.

Uses speech-to-text followed by an LLM pass for executive summary and action items.

## Stack

- **Backend:** Python 3.11+, FastAPI, Uvicorn
- **AI:** OpenAI Whisper (transcription), OpenAI `gpt-4o-mini` (summarization)
- **Frontend (optional demo UI):** React + Vite

## Features

- Audio upload (`.mp3`, `.wav`, `.m4a`)
- Full transcript generation
- Executive summary, takeaways, and action items

## Quick start

```bash
cd backend
python3 -m venv venv
source venv/bin/activate
pip install -r requirements.txt
cp .env.example .env   # set OPENAI_API_KEY
uvicorn main:app --reload --port 8005
```

API docs: http://localhost:8005/docs

```bash
cd frontend
npm install
npm run dev
```

## Author

Pooja Sharma — [Pooja101117](https://github.com/Pooja101117)
