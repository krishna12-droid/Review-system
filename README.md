# 💬 Sentiment Analyzer: Wonders & Restaurants

This Python project is an interactive **opinion miner** that performs **sentiment analysis** on reviews of **Wonders of the World** and **popular restaurant chains** using **NLTK's VADER** sentiment analyzer. It allows users to explore existing reviews, analyze overall sentiment, and contribute their own feedback — all saved locally in JSON files.

---

## 🚀 Features

- 🧠 Sentiment analysis using **VADER** from NLTK
- 💾 Stores and updates reviews in local **JSON** files
- 📊 Analyzes the average sentiment of multiple reviews
- 👤 Interactive CLI for personalized conversations
- 🔁 Allows users to **add and review multiple times**

---

## 🧱 Technologies Used

| Component         | Technology          |
|------------------|---------------------|
| Language          | Python 3.x          |
| NLP               | NLTK + VADER        |
| Storage           | JSON file I/O       |
| Interaction       | Command Line (CLI)  |

---

## 📁 File Structure

.
├── sentiment_analyzer.py # Main Python script (your code)
├── reviews_wonders.json # Predefined reviews of wonders (auto-generated if missing)
├── reviews_restaurants.json # Predefined reviews of restaurants (auto-generated if missing)
└── README.md # This documentation file

yaml
Copy
Edit

---

## 📥 Installation

### 1. Clone the repository

```bash
git clone https://github.com/your-username/sentiment-analyzer.git
cd sentiment-analyzer
2. Create virtual environment (optional but recommended)
bash
Copy
Edit
python -m venv venv
source venv/bin/activate  # or venv\Scripts\activate on Windows
3. Install dependencies
bash
Copy
Edit
pip install nltk
4. Download NLTK resources
bash
Copy
Edit
python
>>> import nltk
>>> nltk.download('vader_lexicon')
>>> exit()
🧪 How to Run
bash
Copy
Edit
python sentiment_analyzer.py
You’ll be greeted with a friendly conversation asking for your name, day, and interests. From there, you can:

Choose between Wonders of the World or Restaurants

Pick a topic from a list

View existing reviews and their sentiment

Submit your own review

See live sentiment analysis results

📈 How Sentiment Works
The VADER sentiment analyzer returns a compound score for each review between -1.0 (very negative) and +1.0 (very positive).

Your script:

Averages all compound scores for a topic

Outputs whether the overall sentiment is positive, negative, or neutral

Shows sentiment for each individual review

✍️ Example Interaction
vbnet
Copy
Edit
Hello! I'm your opinion miner. How are you today?
What's your name?
> Alex
Nice to meet you, Alex!
How's your day going?
> Pretty good!
What's the best part of your day so far?
> Lunch with friends.

Which type of review would you like to explore?
1. Wonders of the World
2. Restaurants
> 2

Which one would you like to know about?
1. McDonald's
2. KFC
...

Most people have a positive opinion about McDonald's.

Do you have any other concerns about this place?
> Yes
Please enter your review:
> The burgers were cold and the service was slow.
...
💾 Persistent Data
All new reviews are appended to either reviews_wonders.json or reviews_restaurants.json.

These files are auto-created if missing and saved automatically after each interaction.

📌 Notes
Supports infinite feedback loops for continued review & sentiment analysis

Designed for educational, NLP demo, or basic chatbot purposes

No internet/API access required

