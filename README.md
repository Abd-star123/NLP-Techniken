Consumer Complaints NLP Analysis
📋 Project Overview
This project implements a comprehensive NLP analysis of consumer complaints from the CFPB dataset using topic modeling techniques. The analysis identifies key themes in consumer complaints through Latent Dirichlet Allocation (LDA) and Non-Negative Matrix Factorization (NMF) methods.

🎯 Key Features
Data Preprocessing: Text cleaning, tokenization, and stopword removal

Topic Modeling: Implementation of both LDA and NMF algorithms

Comparative Analysis: Side-by-side comparison of LDA vs NMF results

📊 Results Summary
Optimal Topics: 2 topics identified

Coherence Score: 0.5815

Topic Distribution:

Topic 1: 470 documents (9.4%) - Focus on claims, reporting, and collections

Topic 2: 4527 documents (90.6%) - Focus on accounts, credit, and consumer reports

🛠️ Installation & Setup
Prerequisites
Python 3.7+



# Download necessary NLTK data
import nltk
nltk.download('stopwords')
nltk.download('punkt')

# Download spaCy model
!python -m spacy download en_core_web_sm
🚀 How to Run
Option 1: Google Colab (Recommended)
Upload the notebook to Google Colab

Run all cells sequentially

The dataset will be automatically downloaded from Kaggle

Option 2: Local Jupyter Notebook
Ensure all dependencies are installed

Download the dataset manually from Kaggle

Update the file path in the notebook to point to your local dataset

Run all cells

🔧 Code Sections
1. Data Loading & Exploration
Loads CFPB consumer complaints dataset

Basic data exploration and cleaning

2. Text Preprocessing
Text cleaning (lowercasing, punctuation removal)

Stopword filtering

Tokenization

3. Topic Modeling Preparation
Dictionary and corpus creation

TF-IDF vectorization

4. Optimal Topic Determination
Coherence score calculation for topics 2-7

Visualization of coherence scores

Selection of optimal topic count

5. Model Training
LDA model training with optimal topics

NMF model training

Topic keyword extraction

6. Results Analysis
Side-by-side topic comparison

Topic distribution analysis

Results export to text files

📈 Output Files
Generated Files:
topic_keywords.txt: Contains optimal topic count, coherence score, and keywords from both LDA and NMF models

Coherence score plot: Visual representation of topic optimization

Key Metrics:
Coherence Score: 0.5815 (indicates good topic quality)

Optimal Topics: 2

Model Comparison: LDA and NMF show consistent topic identification

🎪 Identified Topics
Topic 1: Claims & Collections (9.4%)
Keywords: claim, reporting, collection, debt, compliance, plaintiff

Topic 2: Accounts & Credit Reports (90.6%)
Keywords: account, credit, consumer, report, information, deletion, qualified, entry

📝 Interpretation
The analysis reveals two dominant themes in consumer complaints:

Financial Claims & Legal Issues: Focus on debt collection, compliance, and legal proceedings

Account Management & Credit Reporting: Dominant theme covering credit reports, account information, and data management issues

🔍 Technical Details
Algorithms Used:
LDA (Latent Dirichlet Allocation): Probabilistic topic modeling

NMF (Non-Negative Matrix Factorization): Matrix decomposition approach


Parameters:
Topics Tested: 2-7

Optimal Topics: 2 (based on highest coherence score)

LDA Passes: 15

TF-IDF Features: 2000 maximum featuresbuting
