# 🎧 Multi-Label Emotion Classification for Song Lyrics using Groq + LLaMA 3

This project uses the **Groq API** with the **LLaMA 3 (70B)** model to label song lyrics with 2–4 dominant emotions. It's optimized for emotion-aware music analysis, curation, and dataset enrichment.

---

## 🧠 What This Script Does

- Reads lyrics from a CSV file (`good.csv`)
- Sends each lyric to the **LLaMA3 model via Groq's OpenAI-compatible endpoint**
- Receives **2–4 emotional labels** (from a fixed list of 12)
- Saves the labeled data to a new CSV

---

## 💬 Emotion Categories

The model selects from:

> **joy, anger, fear, nostalgia, sad, obsession, sexual, hope, calm, tender, violence, power**

---

## 📂 Input CSV Requirements

- File name: `good.csv`
- Must contain a `lyrics` column
- The script will automatically create and fill an `emotions` column

---

## ⚙️ Setup Instructions

### 1. Install dependencies

```bash
pip install pandas requests
