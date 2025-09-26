# Text-Analysis-Project-for-youtube-comments
Topic modelling analysis using NMF and apply bigrams and trigrams also generated word cloud

YouTube Comments Text Analysis
📌 Project Overview

This project demonstrates how to analyze YouTube comments using Natural Language Processing (NLP).
It covers:

Data preprocessing (cleaning, tokenization, stopword removal).

Feature extraction with TF-IDF.

Topic Modeling using Non-Negative Matrix Factorization (NMF).

Word Clouds for each topic.

Bigram & Trigram frequency analysis.

Dataset used: Synthetic dataset of 1000 YouTube comments (simulating real-world YouTube video comments).

🛠️ Tech Stack

Python 3.8+

Libraries:

pandas – Data handling

nltk – Tokenization & stopwords

scikit-learn – TF-IDF & NMF topic modeling

matplotlib – Visualization

wordcloud – Word cloud generation

collections – N-gram frequency analysis

📂 Project Workflow

Load Data

df = pd.read_excel("youtube_comments_1000.xlsx")


Preprocessing Steps

Drop missing values.

Convert text to lowercase.

Remove special characters.

Tokenize comments.

Remove stopwords.

Topic Modeling with NMF

Convert processed text to TF-IDF features.

Apply NMF to extract n topics.

Display top words for each topic.

Word Cloud Visualization

Generate word clouds per topic using word importance.

Bigram & Trigram Analysis

Extract most common 2-word and 3-word combinations.

Display top 20 bigrams & trigrams.

📊 Example Outputs

Topic Keywords (sample):

Topic #1: love amazing best vocals talent
Topic #2: video audio quality better expected
...


Word Clouds – Each topic is visualized with a word cloud.

Top Bigrams (Sample):

Bigram	Frequency
love video	35
amazing song	28
🚀 How to Run

Clone the repository

git clone https://github.com/your-username/youtube-comments-nlp.git
cd youtube-comments-nlp


Install dependencies

pip install -r requirements.txt


Run the script

python analysis.py

📦 Requirements

Create a requirements.txt with:

pandas
nltk
scikit-learn
matplotlib
wordcloud
openpyxl

📌 Future Improvements

Integrate with YouTube API to fetch real comments dynamically.

Add BERTopic / LDA models for comparison.

Sentiment analysis (VADER / TextBlob).

Dashboard using Streamlit.
