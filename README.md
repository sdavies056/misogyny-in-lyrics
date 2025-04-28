# misogyny-in-lyrics
Data Science in Economics (BEE2041) - Empirical Project

GitHub Repository: https://github.com/sdavies056/misogyny-in-lyrics

# Project Overview
This project analyses misogynistic language in Billboard Top 50 songs over 50 years (1972–2021) using:

Web scraping (Genius API for lyrics)
Sentiment analysis (TextBlob, VADER)
Term frequency analysis (regex-based misogynistic word counts)

Requirements
Python Packages
Install dependencies via:
bash
pip install pandas lyricsgenius textblob vaderSentiment wordcloud matplotlib seaborn fuzzywuzzy 
API Access
Sign up for a Genius API token.

Replace the placeholder in config.py:
python
GENIUS_API_TOKEN = "YOUR_TOKEN_HERE"

Data Sources
Billboard Top 50 Year-End Charts (1972–2021):
https://www.kaggle.com/datasets/liquidgenius1/billboard-yearend-hot-100-singles-usa
File: Full_Billboard_year_end_hot_100_USA.csv (included in data/Raw/).
Lyrics: Fetched using Genius API (saved to data/Processed/lyrics_*.json).

# Reproduction Steps
Remember to:
bash
 git status
 git add .
 git push origin main

Data Collection:
Run notebooks/misogyny-in-lyrics.ipynb to:

Scrape lyrics (requires Genius API token).
Clean and merge datasets.
*Ensure to read my comments as if i were to repeat this I would certainly not run the exact same code
In hindsight, I made an awful lot of mistakes and should have been alot more thoughtful in order for this 
to run smoothly and efficiently. 

Analysis & Visuals
Run notebooks/misogyny-in-lyrics.ipynb for:

Sentiment analysis (TextBlob/VADER).
Misogynistic word counts.
Temporal trends (line plots).
Word clouds and bar charts.

Outputs
Blog Post: Link to hosted version or see blog.ipynb.

Key Visualizations:
figures/sentiment_trends.png: Yearly sentiment scores.
figures/wordcloud_*.png: Decadal word frequencies.

# Limitations
Missing Lyrics: 100 songs (4%) had no lyrics available.
Some songs will have been assigned incorrect lyrics. 
Language Bias: Non-English lyrics may be miscounted.
Term Subjectivity: "Misogynistic" terms were manually defined.


# Reflection 
I found this project challenging. Due to some unfortunate blunders it was made harder than it should've been, 
however whilst trying to resolve these I do feel as though I have learned alot and would feel quite comfortable 
attempting something similar. I'm happy with how I troubleshooted and attempted to diagnose problems and consequently
solve them, it took some out-of-the box thinking which was painstaking at times but naturally very rewarding. It was also
quite a fun project to do, and I would happily carry out some further exploration at a later date. 