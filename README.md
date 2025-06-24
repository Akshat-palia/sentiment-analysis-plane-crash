# ✈️ Sentiment Analysis on Ahmedabad Plane Crash Tweets

This project performs real-time **sentiment analysis** on tweets related to the **Ahmedabad plane crash**, classifying them as **Positive**, **Negative**, or **Neutral**. It also visualizes the sentiment distribution and auto-generates a PDF report — creating a complete, end-to-end NLP pipeline using Python.

![Pie Chart](sentiment_pie_chart.png)

---

## 📌 Project Overview

🔍 The goal is to extract public sentiment from Twitter to:
- Understand how people reacted to a major real-world event
- Practice real-world data scraping, NLP, and data visualization
- Build a full data pipeline from raw data to visual reports

---

## 🧰 Tech Stack & Tools Used

| Area               | Tools / Libraries                                   |
|--------------------|-----------------------------------------------------|
| 🐍 Programming     | Python 3                                             |
| 🔌 API Access      | [Tweepy](https://www.tweepy.org/) (Twitter API)     |
| 💬 NLP             | [VADER](https://github.com/cjhutto/vaderSentiment), [TextBlob](https://textblob.readthedocs.io/) |
| 📊 Visualization   | Matplotlib                                          |
| 📄 Report Gen      | ReportLab (PDF generation)                          |
| 🔐 Security        | `.env` with `python-dotenv`                         |
| 📁 Git/GitHub      | Version control & public project hosting            |

---

## 📂 Project Structure

```plaintext
sentiment_analysis/
├── fetch_tweets.py                  # Fetches tweets using Twitter API
├── analyze_sentiment.py            # Sentiment analysis using VADER
├── analyze_sentiment_textblob.py   # Sentiment analysis using TextBlob
├── sentiment_summary.py            # Summarizes sentiment counts
├── sentiment_visualization.py      # Creates bar & pie charts
├── generate_pdf_report.py          # Compiles PDF with summary and charts
│
├── tweets.txt                      # Raw fetched tweets
├── sentiment_results.txt           # VADER sentiment output
├── sentiment_results_textblob.txt  # TextBlob sentiment output
├── sentiment_report.pdf            # Final PDF report
├── sentiment_analysis_phases_report.pdf  # Process documentation
│
├── sentiment_pie_chart.png         # Pie chart image
├── sentiment_bar_chart.png         # Bar chart image
│
├── .gitignore                      # Excludes .env and pycache
└── README.md                       # You're here!
