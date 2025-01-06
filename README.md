### ✂️ Text Summarizer ✨  

A **simple and efficient text summarizer** built using **NLTK (Natural Language Toolkit)** for natural language processing. This tool helps you condense lengthy text into short, meaningful summaries by identifying and extracting the most relevant sentences.  

---

## 🚀 Features  
- 🔍 **Sentence Tokenization:** Splits the input text into individual sentences for accurate processing.  
- 📊 **Word Frequency Analysis:** Highlights the most important words in the text while ignoring stop words and punctuation.  
- 📝 **Sentence Scoring:** Assigns scores to sentences based on word frequencies and normalizes by sentence length.  
- ✨ **Summary Generation:** Extracts top-scoring sentences to generate a concise and meaningful summary.  

---

## 🛠️ Requirements  
- 🐍 Python 3.x  
- 📚 NLTK library  

---

## 📥 Installation  

1. Clone the repository:  
   ```bash
   git clone https://github.com/your-username/text-summarizer.git
   cd text-summarizer
   ```

2. Install dependencies:  
   ```bash
   pip install nltk
   ```

3. Download the required NLTK data:  
   ```python
   import nltk
   nltk.download('punkt')
   nltk.download('stopwords')
   ```

---

## ⚡ Usage  

### Example Code:  

```python
from nltk.tokenize import word_tokenize, sent_tokenize
from nltk.corpus import stopwords
from collections import defaultdict
from string import punctuation

# Define text for summarization
text = """
Machine learning is a field of artificial intelligence that focuses on the use of data and algorithms to imitate the way that humans learn, gradually improving its accuracy. Machine learning is an important component of the growing field of data science. Through the use of statistical methods, algorithms are trained to make classifications or predictions, uncovering key insights within data mining projects. These insights subsequently drive decision making within applications and businesses, ideally impacting key growth metrics. As big data continues to expand and grow, the market demand for data scientists will increase. They will be required to help identify the most relevant business questions and subsequently the data to answer them.
"""

# Generate summary
summary = summarize_text(text, num_sentences=2)
print("Original Text:")
print(text)
print("\nSummary:")
print(summary)
```

### Output:  
📜 **Original Text:**  
> Machine learning is a field of artificial intelligence that focuses on the use of data and algorithms to imitate the way that humans learn, gradually improving its accuracy. Machine learning is an important component of the growing field of data science...  

✨ **Summary:**  
> Machine learning is an important component of the growing field of data science. As big data continues to expand and grow, the market demand for data scientists will increase.  

---

## 🧩 Functions  

### 1. `create_frequency_table(text)`  
🛠️ Creates a frequency table for the words in the input text.  
- **Input:** Text string  
- **Output:** Dictionary with word frequencies  

### 2. `score_sentences(sentences, freq_table)`  
📊 Scores each sentence based on the frequency of important words.  
- **Input:** List of sentences, frequency table  
- **Output:** Dictionary with sentence scores  

### 3. `summarize_text(text, num_sentences=3)`  
✨ Summarizes the input text by extracting top-scoring sentences.  
- **Input:** Text string, number of sentences for the summary  
- **Output:** Concise summary  

---

## 🎯 Testing the Summarizer  

### Example Input:  
```python
your_text = """
Elasticsearch is an open source distributed, RESTful search and analytics engine, scalable data store, and vector database capable of addressing a growing number of use cases. As the heart of the Elastic Stack, it centrally stores your data for lightning-fast search, fine‑tuned relevancy, and powerful analytics that scale with ease.
"""
summary = summarize_text(your_text, num_sentences=2)
print(summary)
```

### Example Output:  
✨ **Summary:**  
> Elasticsearch is an open source distributed, RESTful search and analytics engine, scalable data store, and vector database capable of addressing a growing number of use cases. As the heart of the Elastic Stack, it centrally stores your data for lightning-fast search, fine-tuned relevancy, and powerful analytics that scale with ease.  

---

## 🌟 Contributing  
We ❤️ contributions!  
- Fork the repository  
- Make your changes  
- Submit a pull request ✨  

---

## ❗ License  
This project is **not licensed yet.** If you wish to use it, please contact the repository owner for permissions.  

---

🚀 Happy Summarizing! 🎉  
