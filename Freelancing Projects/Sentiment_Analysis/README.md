XYZ COMPANY NLP & Text Analysis


📌 Project Overview

This project was completed as part of the XYZ Data Extraction and NLP Assignment.
The objective was to:

Extract textual data from 147 article URLs.

Perform sentiment analysis and readability analysis using the provided Master Dictionary and StopWords lists.

Generate structured output in Final_Output.xlsx following the given template.

⚙️ Methodology
🔹 Data Extraction

Loaded URLs from Input.xlsx.

Scraped article title and body text using requests and BeautifulSoup.

Saved each article in a text file (<URL_ID>.txt) and archived into Articles.zip.

🔹 Data Cleaning

Converted text to lowercase.

Removed punctuation, numbers, and special characters (regex).

Removed stopwords using the provided StopWords folder.

🔹 Text Analysis

Calculated the following metrics for each article:

Sentiment Analysis

Positive Score

Negative Score

Polarity Score

Subjectivity Score

Readability Metrics

Average Sentence Length

Percentage of Complex Words

Fog Index

Average Words per Sentence

Word-Level Metrics

Complex Word Count

Word Count

Syllables per Word

Personal Pronouns

Average Word Length

🔹 Output Generation

Final results saved into Final_Output.xlsx.

Extracted articles saved in Articles.zip.

🛠️ How to Run

Install dependencies

pip install pandas requests beautifulsoup4 nltk openpyxl


Download NLTK resources (first time only):

import nltk
nltk.download('punkt')
nltk.download('punkt_tab')


Ensure required files are available

assignment.py

Input.xlsx

Output Data Structure.xlsx

StopWords folder

positive-words.txt

negative-words.txt

Run the script

python assignment.py


Generated outputs

Final_Output.xlsx → Sentiment & readability metrics

Articles.zip → Extracted text files

📂 Project Structure
📦 XYZ-NLP-Analysis
 ┣ 📜 assignment.py
 ┣ 📜 Input.xlsx
 ┣ 📜 Output Data Structure.xlsx
 ┣ 📜 positive-words.txt
 ┣ 📜 negative-words.txt
 ┣ 📂 StopWords
 ┣ 📜 Final_Output.xlsx
 ┣ 📜 Articles.zip
 ┗ 📜 Instructions.docx

🚀 Tech Stack

Python 3.9+

Libraries: pandas, requests, beautifulsoup4, nltk, openpyxl, regex, zipfile

📑 Deliverables

assignment.py → Main script

Final_Output.xlsx → Results file

Articles.zip → Extracted articles

Instructions.docx → Documentation
