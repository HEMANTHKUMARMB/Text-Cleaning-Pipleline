# 🧹 NLP Text Cleaning Pipeline

## 📌 Project Overview

This project demonstrates different **Natural Language Processing (NLP) text preprocessing techniques** using Python.

The project focuses on cleaning raw text from:

1. Customer Reviews
2. Social Media Comments
3. Customer Review Datasets
4. News Articles

Text cleaning is an important step in NLP because real-world text often contains uppercase letters, punctuation, special characters, stopwords, contractions, hashtags, mentions, emojis, and unnecessary spaces.

---

## 🎯 Objective

The main objective of this project is to build Python-based NLP preprocessing pipelines that transform raw text into clean and useful text for further analysis or machine learning.

---

## 🛠️ Technologies Used

* Python
* Google Colab / Jupyter Notebook
* Pandas
* NLTK
* Regular Expressions (`re`)
* Contractions Library
* Collections (`Counter`)

---

# 📚 Practical Tasks

## Task 1: Text Cleaning Pipeline

A text-cleaning pipeline is created for customer reviews.

### Preprocessing Steps

* Case Folding
* Special Character Removal
* Stopword Removal
* Contraction Expansion
* Extra Space Removal
* Word Count Before Cleaning
* Word Count After Cleaning
* Comparison of Original and Cleaned Text

### Example

**Original:**

`I'm really HAPPY about this product!!! It's amazing & I don't think I've ever used something this good.`

**Cleaned:**

`really happy product amazing think ever used something good`

---

## Task 2: Social Media Text Cleaning

Social media comments usually contain hashtags, mentions, emojis, punctuation, and informal language.

### Preprocessing Steps

* Case Folding
* Contraction Expansion
* Hashtag Removal
* Mention Removal
* Emoji and Special Character Removal
* Stopword Removal
* Extra Space Removal
* Before and After Comparison

### Example

**Original:**

`OMG!!! I can't believe this 😍 @user #Amazing`

**Cleaned:**

`omg cannot believe`

---

## Task 3: Customer Review Preprocessing

This task preprocesses a dataset containing **100 customer reviews**.

### Operations Performed

* Convert reviews to lowercase
* Expand contractions
* Remove special characters
* Remove stopwords
* Remove unnecessary whitespace
* Create a new `cleaned_review` column
* Calculate word count before cleaning
* Calculate word count after cleaning
* Compare average word counts
* Identify the 10 most frequent words

### Dataset Structure

| Column           | Description                     |
| ---------------- | ------------------------------- |
| `review`         | Original customer review        |
| `cleaned_review` | Preprocessed customer review    |
| `words_before`   | Number of words before cleaning |
| `words_after`    | Number of words after cleaning  |

### Top 10 Frequent Words

Python's `Counter` class is used to identify the 10 most frequently occurring words in the cleaned customer reviews.

---

## Task 4: News Article Text Cleaning

This task preprocesses **20 news articles**.

### Preprocessing Steps

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

# 🔄 NLP Preprocessing Workflow

```text
Raw Text
   ↓
Contraction Expansion
   ↓
Case Folding
   ↓
Remove Hashtags / Mentions (when required)
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
Text Analysis / Machine Learning
```

---

# 📦 Installation

Install the required Python libraries:

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
5. Run each cell one by one.
6. View the original and cleaned text outputs.

### Jupyter Notebook

Install the required packages:

```bash
pip install pandas nltk contractions
```

Then start Jupyter Notebook:

```bash
jupyter notebook
```

Open the project notebook and run the cells.

---

# 📂 Suggested Project Structure

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

# 📊 Expected Results

After preprocessing:

* Text is converted to lowercase.
* Contractions are expanded.
* Unnecessary punctuation and special characters are removed.
* Stopwords are removed.
* Extra whitespace is removed.
* Social media hashtags and mentions are removed when required.
* Original and cleaned text can be compared.
* Average word counts can be calculated.
* Frequent words can be identified.

---

# 💡 Applications

Text preprocessing can be used in:

* Sentiment Analysis
* Customer Feedback Analysis
* Social Media Analysis
* News Classification
* Spam Detection
* Text Classification
* Recommendation Systems
* Chatbots
* Machine Learning
* Natural Language Processing

---



## 👨‍💻 Project Information

**Project:** Text Cleaning Pipeline
**Type:** Practical Task
**Batch:** Data Science MITM

