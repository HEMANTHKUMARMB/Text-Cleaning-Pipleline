# 🧹 NLP Text Cleaning Pipeline

## 📌 Project Overview

This project demonstrates a complete **Natural Language Processing (NLP) Text Cleaning Pipeline** using Python.

The project cleans different types of text, including:

* Customer Reviews
* Social Media Comments
* Customer Review Datasets
* News Articles

Text preprocessing removes unnecessary information and prepares raw text for machine learning and NLP applications.

---

# 🎯 Project Objectives

The main objectives are:

1. Convert text to lowercase using case folding.
2. Expand contractions.
3. Remove special characters.
4. Remove stopwords.
5. Remove unnecessary whitespace.
6. Remove hashtags and mentions where required.
7. Compare text before and after preprocessing.
8. Calculate word counts.
9. Identify frequent words.
10. Measure text-size reduction.

---

# 🛠️ Technologies Used

* Python
* Google Colab / Jupyter Notebook
* Pandas
* NLTK
* Regular Expressions (`re`)
* Contractions
* Collections (`Counter`)

---

# 📚 Practical Tasks

## Practical Task 1: Text Cleaning Pipeline

A text-cleaning pipeline is created to preprocess customer reviews.

### Techniques

* Case Folding
* Special Character Removal
* Stopword Removal
* Contraction Expansion
* Extra Space Removal
* Word Count Comparison

### Example

**Original Text:**

`I'm really HAPPY about this product!!! It's amazing & I don't think I've ever used something this good.`

**Cleaned Text:**

`really happy product amazing think ever used something good`

---

# 📱 Practical Task 2: Social Media Text Cleaning

Social media comments contain hashtags, mentions, emojis, punctuation, contractions, and unnecessary characters.

### Techniques

* Case Folding
* Contraction Expansion
* Hashtag Removal
* Mention Removal
* Special Character Removal
* Emoji Removal
* Stopword Removal
* Extra Space Removal

### Example

**Before:**

`OMG!!! I can't believe this 😍 @user #Amazing`

**After:**

`omg cannot believe`

---

# ⭐ Practical Task 3: Customer Review Preprocessing

A dataset containing **100 customer reviews** is processed.

### Steps

1. Convert text to lowercase.
2. Expand contractions.
3. Remove special characters.
4. Remove stopwords.
5. Remove unnecessary whitespace.
6. Create a `cleaned_review` column.
7. Count words before preprocessing.
8. Count words after preprocessing.
9. Calculate average word counts.
10. Identify the 10 most frequent words.

### Dataset Structure

| Column           | Description                     |
| ---------------- | ------------------------------- |
| `review`         | Original customer review        |
| `cleaned_review` | Cleaned customer review         |
| `words_before`   | Number of words before cleaning |
| `words_after`    | Number of words after cleaning  |

---

# 📰 Practical Task 4: News Article Text Cleaning

A collection of **20 news articles** is processed using NLP preprocessing.

### Techniques

* Case Folding
* Contraction Handling
* Special Character Removal
* Stopword Removal

### Example

**Original:**

`Scientists can't confirm the results yet, but the research looks promising.`

**Cleaned:**

`scientists cannot confirm results yet research looks promising`

---

# 🔄 NLP Preprocessing Pipeline

```text
Raw Text
    ↓
Contraction Expansion
    ↓
Case Folding
    ↓
Remove Hashtags / Mentions
    ↓
Remove Special Characters
    ↓
Remove Extra Spaces
    ↓
Tokenization
    ↓
Stopword Removal
    ↓
Cleaned Text
    ↓
Word Frequency Analysis
    ↓
Final NLP Dataset
```

---

# 📊 Text Analysis

After preprocessing the text, the following questions are analyzed.

---

## 1. How Many Words Were Present Before Preprocessing?

### Definition

Words before preprocessing represent the **total number of words available in the original/raw text before text cleaning**.

### Formula

```text
Words Before = Total number of words in original text
```

### Python

```python
words_before = len(original_text.split())
```

### Example

If the original dataset contains 200 words:

```text
Words Before = 200
```

---

## 2. How Many Words Remained After Preprocessing?

### Definition

Words after preprocessing represent the **number of words remaining after stopwords, punctuation, special characters, and other unnecessary information have been removed**.

### Formula

```text
Words After = Total number of words in cleaned text
```

### Python

```python
words_after = len(cleaned_text.split())
```

### Example

```text
Words Before = 200
Words After  = 120
```

Therefore, 120 useful words remain after preprocessing.

---

## 3. Which 10 Words Occur Most Frequently?

### Definition

Word frequency represents the **number of times a particular word appears in the cleaned text**.

The 10 words with the highest occurrence counts are called the **Top 10 Most Frequent Words**.

### Formula

```text
Frequency(word) = Number of times the word occurs
```

### Python

```python
from collections import Counter

word_frequency = Counter(cleaned_text.split())

top_10_words = word_frequency.most_common(10)

print(top_10_words)
```

### Example

| Word       | Frequency |
| ---------- | --------: |
| product    |        25 |
| good       |        20 |
| quality    |        18 |
| company    |        15 |
| market     |        13 |
| new        |        12 |
| service    |        10 |
| technology |         9 |
| customer   |         8 |
| delivery   |         7 |

---

## 4. Which Stopwords Appeared Most Frequently?

### Definition

**Stopwords** are commonly occurring words that usually provide little information for many NLP tasks.

Examples include:

`the`, `is`, `a`, `an`, `and`, `of`, `to`, `in`, `was`, `this`

The most frequent stopwords are the stopwords that occur the greatest number of times in the original text.

### Formula

```text
Stopword Frequency =
Number of times a stopword occurs in the original text
```

### Python

```python
from collections import Counter

stopword_frequency = Counter(found_stopwords)

top_stopwords = stopword_frequency.most_common(10)

print(top_stopwords)
```

---

## 5. How Much Did the Text Size Reduce?

### Definition

Text-size reduction measures **how much unnecessary text was removed during preprocessing**.

### Words Removed Formula

```text
Words Removed = Words Before - Words After
```

### Percentage Reduction Formula

```text
Reduction % =
((Words Before - Words After) / Words Before) × 100
```

### Example

Suppose:

```text
Words Before = 200
Words After  = 120
```

Words removed:

```text
200 - 120 = 80 words
```

Percentage reduction:

```text
((200 - 120) / 200) × 100

= (80 / 200) × 100

= 0.4 × 100

= 40%
```

Therefore:

**Words Removed = 80**

**Text Size Reduction = 40%**

---

# 📋 Formula Summary

| Analysis           | Formula / Method                       |
| ------------------ | -------------------------------------- |
| Words Before       | `len(original_text.split())`           |
| Words After        | `len(cleaned_text.split())`            |
| Words Removed      | `Words Before - Words After`           |
| Word Frequency     | Number of occurrences of each word     |
| Top 10 Words       | `Counter(words).most_common(10)`       |
| Stopword Frequency | Number of occurrences of each stopword |
| Reduction %        | `((Before - After) / Before) × 100`    |

---

# 📦 Installation

Install the required Python packages:

```bash
pip install pandas nltk contractions
```

---

# ▶️ How to Run

### Google Colab

1. Open Google Colab.
2. Create a new notebook.
3. Copy the project code into the notebook.
4. Install the required libraries.
5. Run each cell from top to bottom.
6. Check the cleaned text and analysis results.

### Jupyter Notebook

Install the dependencies:

```bash
pip install pandas nltk contractions
```

Start Jupyter:

```bash
jupyter notebook
```

Then open the project notebook and run all cells.

---

# 📂 Project Structure

```text
Text-Cleaning-Pipeline/
│
├── Text_Cleaning_Pipeline.ipynb
├── README.md
└── requirements.txt
```

---

# 📋 requirements.txt

```text
pandas
nltk
contractions
```

---

# 💡 Applications

The preprocessing pipeline can be used for:

* Sentiment Analysis
* Customer Feedback Analysis
* Social Media Analysis
* News Classification
* Spam Detection
* Text Classification
* Topic Modeling
* Recommendation Systems
* Chatbots
* Machine Learning
* Natural Language Processing



## 👨‍💻 Project Information

**Project:** Text Cleaning Pipeline

**Type:** Practical Task

**Batch:** Data Science MITM

