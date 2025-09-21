# Dataset Creator (JSONL) — Browser-Based

A lightweight, browser-based **dataset creator** to build prompt–completion pairs, organize them by category, track simple stats, and export to **JSONL** for LLM fine-tuning.

> **Note**  
> Everything runs **locally in your browser**. No server, no telemetry.  
> The **File System Access API** is used for opening/saving a `.txt` database file (Chromium-based browsers recommended).

## Features
- Add prompt/completion pairs with a **category** and timestamp
- **Stats** per category + total count
- **Pagination** for large datasets
- **Import/Load** from a local text file (line-delimited JSON)
- **Export** to JSONL
- Simple, clean UI (Tailwind + daisyUI)

## Tech Stack
- HTML + Vanilla JS
- TailwindCSS & daisyUI
- File System Access API (Chrome/Edge/Brave)

## Getting Started
1. Open `index.html` in a Chromium-based browser.
2. Click **Open / Create Database** to choose or create your local dataset file.
3. Add examples via the form (prompt, completion, category).
4. Use **Export JSONL** to generate a `dataset.jsonl`.

## Data Format
Each line (JSONL) contains:
```json
{ "prompt": "...", "completion": "...", "category": "cat", "date": "YYYY-MM-DD HH:mm:ss" }
