# Ollama WebNovel to EPUB

A Python-based tool that uses **AI (via Ollama)** to intelligently extract web novel chapters and compile them into clean EPUB files for offline reading.

## 🚀 Features

- ✅ **AI-powered chapter parsing** with [Ollama](https://ollama.com/)
- Extracts title and content directly from raw HTML using a local language model
- 🌐 Scrapes and downloads novel chapters from supported web novel sites
- 📖 Converts chapters into EPUB format with title, metadata, and structure
- 📝 Saves novel metadata (title, author, genre, cover image, etc.)
- 📊 Tracks download and conversion progress in the terminal

## 🧠 Why AI?

Traditional scrapers rely on fragile CSS selectors. This project uses a local LLM (like `llama3` or `tinyllama` running on Ollama) to **understand HTML structure and extract meaningful content**, making it more robust across different web novel sites.


## Disclaimer
Disclaimer: This tool is intended for personal use only. You should only scrape and download content for which you own the rights or have explicit permission from the copyright holder. The developer does not condone or support copyright infringement of any kind.

## Installation
```bash
git clone https://github.com/ShaneMatthews93/ollama_webnovel_to_epub
cd ollama_webnovel_to_epub
pip install -r requirements.txt

## 🧠 AI Setup (Ollama)
To use the AI extraction features, make sure Ollama is installed and running on your server or local machine.

If you’re running Ollama on a separate server, update the ask_llama() function in src/ollama_scraper.py to point to your remote machine’s IP address: