# Notes to Anki

A Streamlit app that turns your reading notes into Anki flashcards using Claude.

## What it does

1. **Paste your notes** — book highlights, study notes, lecture summaries, etc.
2. **Generate flashcards** — Claude reads your notes and creates question/answer pairs
3. **Review & edit** — select which cards to keep, edit the front/back text
4. **Import to Anki** — push directly via AnkiConnect or download a tab-separated file

## Setup

```bash
pip install -r requirements.txt
streamlit run app.py
```

You'll need an [Anthropic API key](https://console.anthropic.com/settings/keys) — enter it in the sidebar.

## Importing to Anki

**Option A: AnkiConnect (direct push)**
1. Install the [AnkiConnect](https://ankiweb.net/shared/info/2055492159) add-on in Anki
2. Keep Anki open while using the app
3. Click "Push to Anki"

**Option B: File import**
1. Download the `.txt` file
2. In Anki: File > Import, select the file, set separator to Tab
