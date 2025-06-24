# 📚 Flash-card-SaaS

An AI-powered Flashcard Generator & Revision Assistant designed to help students learn efficiently using spaced repetition. Upload PDFs or plain text, and the system extracts structured Q\&A pairs and quizzes you in an interactive chatbot interface.

---

## 🚀 Features

* 🧠 **AI-Based Flashcard Generation**: Automatically extract question-answer pairs from educational content (PDF or text).
* 💬 **Interactive Chatbot**: Test your knowledge through a terminal-based quiz loop powered by spaced repetition logic.
* 🗂️ **Spaced Repetition**: Questions reappear based on your answers, helping reinforce weak areas.
* 💾 **Save Flashcards**: Store and load flashcards as structured JSON files for reuse.
* 📾 **PDF/Text Input Support**: Cleanly extract and process content from documents using PyMuPDF.
  
---

## 📦 Installation

```bash
git clone https://github.com/Jai-dayanand/Flash-card-SaaS.git
cd Flash-card-SaaS
pip install -r requirements.txt
```

---

## 📂 Project Structure

```
Flash-card-SaaS/
├── extract.py              # PDF/Text content extractor
├── flashcard_generator.py  # Q&A generation logic
├── spaced_bot.py           # Interactive quiz/chatbot logic
├── chat_flashcard_bot.py   # Main entry point
├── utils/                  # Helper utilities
│   └── preprocessing.py
├── data/
│   └── sample.pdf          # Sample input file
└── flashcards/
    └── output.json         # Generated flashcards
```

---

## 🧪 Usage

### 1. Extract flashcards

```bash
python extract.py data/sample.pdf flashcards/output.json
```

### 2. Start chatbot revision

```bash
python chat_flashcard_bot.py
```

You’ll be quizzed interactively based on your flashcards!

---

## 🧠 Example Flashcard Output (JSON)

```json
[
  {
    "question": "What are the five principal aspects of education?",
    "answer": "Knowledge, wisdom, behavior, character, and creativity.",
    "difficulty": 0,
    "last_seen": "2025-06-24T12:00:00"
  }
]
```

---

## 📌 Roadmap

* [ ] Web-based interface (React + Flask)
* [ ] Flashcard tagging & search
* [ ] User authentication and dashboard
* [ ] Advanced feedback scoring

---

## 🧑‍💻 Author

[Jai Dayanand](https://github.com/Jai-dayanand)

