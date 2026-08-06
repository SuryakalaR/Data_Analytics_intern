# OIBSIP — Data Analytics Track (Suryakala)

This repository contains my completed tasks for the Oasis Infobyte Summer Internship Program (OIB-SIP), Data Analytics track. **7 of the available tasks are complete** (3 from Level 1, 4 from Level 2) — well above the minimum requirement of 3.

---

## Task 1 — Cleaning Data (Level 1)
**Folder:** `DataAnalytics-L1-CleaningData/`

Took a deliberately messy customer dataset (nulls, duplicates, inconsistent text casing, mixed date formats, currency-formatted numbers) and transformed it into a clean, analysis-ready dataset.

**Covers:** data quality report → duplicate removal → text standardisation → dtype correction → justified missing-value handling → IQR-based outlier treatment → before/after summary → exported cleaned CSV.

**Files:** `DataAnalytics_Task1_CleaningData.ipynb`, `messy_customer_data.csv`, `cleaned_customer_data.csv`

---

## Task 2 — EDA on Retail Sales Data (Level 1)
**Folder:** `DataAnalytics-L1-EDARetailSales/`

Exploratory analysis of 6,000 retail orders (2022–2023) across 5 categories and 4 regions to uncover sales patterns and customer behaviour.

**Covers:** monthly/quarterly revenue trends → age/gender demographics → top-10 products → category revenue → correlation heatmap → region×category insight → 3 actionable business recommendations.

**Files:** `DataAnalytics_Task2_EDA_RetailSales.ipynb`, `retail_sales_data.csv`

---

## Task 3 — Sentiment Analysis (Level 1)
**Folder:** `DataAnalytics-L1-SentimentAnalysis/`

NLP classifier distinguishing positive / negative / neutral product reviews (1,800 reviews, ~6% realistic label noise).

**Covers:** preprocessing pipeline → TF-IDF feature extraction → Naive Bayes + Logistic Regression (~94% accuracy) → confusion matrices → WordClouds per class → error analysis on genuine misclassifications → real-world application discussion.

**Files:** `DataAnalytics_Task4_SentimentAnalysis.ipynb`, `product_reviews.csv`

---

## Task 4 — Predicting House Prices with Linear Regression (Level 2)
**Folder:** `DataAnalytics-L2-HousePricePrediction/`

Linear regression model predicting house price from area, bedrooms, bathrooms, age, garage, and location (1,200 listings).

**Covers:** EDA + feature-selection reasoning → missing-value imputation + one-hot encoding → correlation heatmap → Linear Regression (R² ≈ 0.93, RMSE ≈ ₹25,200) → actual-vs-predicted scatter → residual plot → coefficient analysis → bonus Ridge/Lasso comparison.

**Files:** `DataAnalytics_L2Task1_HousePricePrediction.ipynb`, `house_prices.csv`

---

## Task 5 — Fraud Detection (Level 2)
**Folder:** `DataAnalytics-L2-FraudDetection/`

Fraud-detection pipeline on 15,000 transactions with a realistic 2.5% fraud rate.

**Covers:** class-imbalance analysis → amount/time-of-day EDA → why accuracy is misleading here → SMOTE oversampling (train-only) → stratified split → Logistic Regression + Random Forest (Recall ~88–89%, AUC ~0.96–0.97) → ROC curves → precision/recall trade-off discussion → feature importance → scalability discussion (1M transactions/hour).

**Files:** `DataAnalytics_L2Task3_FraudDetection.ipynb`, `credit_card_transactions.csv`

---

## Task 6 — Unveiling the Android App Market (Google Play Store Analysis) (Level 2)
**Folder:** `DataAnalytics-L2-GooglePlayStoreAnalysis/`

Comprehensive analysis of 920 Play Store app listings + 1,531 user reviews.

**Covers:** Installs/Size/Price string cleaning → category saturation analysis → ratings analysis → size-vs-installs correlation → free/paid pricing + revenue-by-category → TextBlob sentiment on reviews → sentiment-by-category → interactive Plotly bubble chart → 3 developer-facing insights.

**Files:** `DataAnalytics_L2Task4_GooglePlayStoreAnalysis.ipynb`, `googleplaystore.csv`, `user_reviews.csv`

---

## Task 7 — Autocomplete and Autocorrect Data Analytics (Level 2)
**Folder:** `DataAnalytics-L2-AutocompleteAutocorrect/`

NLP analysis building and comparing text-prediction and spell-correction systems on a ~51,000-word corpus.

**Covers:** preprocessing + word-frequency visualisation → bigram/trigram autocomplete models → pyspellchecker-based autocorrect (85% accuracy on 20 test misspellings) → Precision/Recall metrics (Autocomplete Recall@3: 100% trigram vs 60% bigram-only; Autocorrect: 85% vs 55% pure-Levenshtein) → limitations vs. production systems (Gboard/Google Keyboard) discussion.

**Files:** `DataAnalytics_L2Task5_AutocompleteAutocorrect.ipynb`, `corpus.txt`

---

## Repository Structure
```
OIBSIP/
├── DataAnalytics-L1-CleaningData/
├── DataAnalytics-L1-EDARetailSales/
├── DataAnalytics-L1-SentimentAnalysis/
├── DataAnalytics-L2-HousePricePrediction/
├── DataAnalytics-L2-FraudDetection/
├── DataAnalytics-L2-GooglePlayStoreAnalysis/
└── DataAnalytics-L2-AutocompleteAutocorrect/
```

Each folder contains its own notebook, dataset(s), and a task-specific `README.md`.

