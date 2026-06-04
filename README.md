# Brexit Immigration Discourse and Toxicity Analysis

## Project Overview

This project investigates immigration-related discourse in YouTube comments published during the Brexit referendum campaign.

Using natural language processing (NLP), semantic embeddings, and toxicity detection models, the analysis identifies comments related to immigration and evaluates the prevalence of hostile or toxic language within online political discussions.

The study combines computational social science methods with machine learning techniques to explore how immigration was discussed by YouTube users during one of the most significant political events in recent British history.

---

## Research Questions

* How frequently was immigration discussed in YouTube conversations related to Brexit?
* Can semantic embeddings automatically identify immigration-related comments?
* What proportion of immigration-related comments exhibit toxic language?
* To what extent does online discussion about immigration contain potentially hostile discourse?

---

## Data Collection

Data were collected using the YouTube Data API.

The workflow included:

* Retrieval of videos from the BBC News playlist "2016 EU Referendum".
* Extraction of video metadata.
* Collection of user comments.
* Data cleaning and preprocessing.

The repository does not include the original comments dataset.

---

## Methodology

The analysis followed four main stages:

### 1. Data Extraction

* YouTube Data API
* Video metadata collection
* Comment extraction

### 2. Semantic Filtering

Immigration-related comments were identified using sentence embeddings generated with Sentence Transformers.

A set of immigration-related reference phrases was used to calculate semantic similarity scores.

Comments with similarity scores above a predefined threshold were classified as immigration-related.

### 3. Toxicity Detection

Toxicity was measured using the Detoxify model.

Each comment received a toxicity score ranging from 0 to 1.

### 4. Exploratory Analysis

* Comment frequencies
* Video engagement metrics
* Toxicity distributions
* Identification of highly toxic comments

---

## Main Results

* More than 3,400 comments were identified as immigration-related.
* Approximately 10% of immigration-related comments were classified as highly toxic.
* The majority of comments exhibited low toxicity levels, although a small subset contained strongly hostile language.
* Semantic embeddings proved effective for identifying immigration-related discourse without relying on keyword matching.

---

## Key Visual Results

### Distribution of Toxicity Levels

![Toxicity Distribution](results/immigration_comments_by_toxicity.png)

### Evolution of YouTube Comments Over Time

![Comments Over Time](results/youtube_comments_over_time.png)

---

## Technologies Used

* Python
* Pandas
* NumPy
* Sentence Transformers
* Hugging Face Transformers
* Detoxify
* YouTube Data API
* Matplotlib
* Seaborn
* Google Colab

---

## Repository Structure

```text
brexit-immigration-discourse-analysis/

│
├── data/
│   └── README.md
│
├── results/
│   ├── README.md
│   ├── youtube_comments_over_time.png
│   └── immigration_comments_by_toxicity.png
│  
├── Brexit_Immigration_Discourse_and_Toxicity_Analysis.ipynb
├── requirements.txt
└── README.md
```

---

## Skills Demonstrated

* API Data Collection
* Natural Language Processing (NLP)
* Semantic Embeddings
* Toxicity Detection
* Computational Social Science
* Social Media Analytics
* Text Mining
* Exploratory Data Analysis

---

## Author

Carlos F. Carreras De León

MSc in Social Data Science

University of Granada
