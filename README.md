# News Headline Analysis of the 2024 US Election

This repository contains the term paper and analysis notebook for the course **Computational Social Science** at **Ludwig Maximilian University of Munich (LMU)**. The project was conducted by **Minh Nguyen** and explores **media framing and sentiment trends** in the 2024 U.S. Presidential Election using computational text analysis methods.

## Project Overview

The U.S. media landscape plays a significant role in shaping public opinion during presidential elections. This study investigates whether systematic differences exist in how left-leaning and right-leaning news outlets covered key political topics leading up to the 2024 U.S. presidential election between Donald Trump and Kamala Harris.

### Research Questions

- Do left- and right-leaning media sources use different emotional tones in headlines?
- How are identical topics (e.g., immigration, Israel-Palestine conflict) framed differently?
- What are the main topics emphasized by each media orientation?

## Data

The dataset was collected from [Media Cloud](https://mediacloud.org), comprising over **7600 headlines** from 8 news outlets (4 left-leaning and 4 right-leaning), dated **January 15 – November 5, 2024**.

- Left-leaning: NYTimes, CNN, The Nation, LA Times  
- Right-leaning: Fox News, NY Post, Breitbart, Hot Air

## Techniques Used

This project combined multiple Natural Language Processing (NLP) techniques:

### 1. **Data Preprocessing**
- Tokenization, stop-word removal (with custom domain-specific list)
- Lemmatization using NLTK’s `WordNetLemmatizer`
- Synonym mapping for consistency across political terminology

### 2. **Sentiment Analysis**
- **NRC Emotion Lexicon**: Multi-label classification of emotions (joy, anger, fear, etc.)
- **AFINN Lexicon**: Scoring headlines on a continuous sentiment scale (-5 to +5)

### 3. **Keyword & Framing Analysis**
- **TF-IDF**: Highlighted key terms unique to each media orientation
- **Bigram Extraction**: Analyzed common phrase structures
- **Word Correlation Analysis**: Examined contextual co-occurrence patterns

### 4. **Topic Modeling**
- **Latent Dirichlet Allocation (LDA)** to discover latent themes in the corpus
- Compared topic distribution across left- and right-leaning outlets

## Key Findings

- **Sentiment Trends**: Right-leaning outlets had more negative sentiments near election day, especially with fear-related emotions.
- **Framing Differences**: 
  - Immigration was framed as humanitarian by left-leaning outlets, and as a national security threat by right-leaning ones.
  - Israel-Palestine coverage reflected sympathetic tones toward Palestine in left media, while right media focused on pro-Israel and anti-Hamas narratives.
- **Topic Modeling**: 
  - Left media emphasized social issues and protests.
  - Right media focused more on immigration and the economy.

## Files

- `nguyen_minh_code.ipynb`: Jupyter Notebook containing code for preprocessing, analysis, and visualization.
- `Submitted paper.pdf`: Full academic write-up including methodology, figures, results, and references.

## Author

Minh Nguyen  
Master’s Student in Data Science  
LMU Munich

---

📘 For detailed figures and in-depth discussion, please see the full paper in `Submitted paper.pdf`.

🧠 This project demonstrates how computational methods can provide insight into political discourse and media framing in polarized environments.
