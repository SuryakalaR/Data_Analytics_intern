# Data Analytics — Task (Level 2): Autocomplete and Autocorrect Data Analytics

**Objective:** Analyse the efficiency and accuracy of autocomplete and autocorrect algorithms using NLP techniques, implementing and comparing multiple approaches for text prediction and spelling correction.

## Files
- `DataAnalytics_L2Task5_AutocompleteAutocorrect.ipynb` — full notebook
- `corpus.txt` — ~51,000-word synthetic text corpus used to build the n-gram frequency model

## What the notebook covers
1. NLP preprocessing (lowercase, punctuation removal, tokenisation, stopword removal for frequency viz)
2. Top-20 most frequent word visualisation
3. Autocomplete: frequency-based bigram + trigram (with backoff) next-word prediction models
4. Tested on 10 input prefixes, top-3 predictions shown for each
5. Autocorrect: edit-distance + frequency-based correction via `pyspellchecker`
6. Tested on 20 deliberately misspelled words — 85% correction accuracy
7. Precision/Recall metrics for both systems (Autocomplete Recall@3: 100% trigram vs 60% bigram-only; Autocorrect Precision 1.0 / Recall 0.85)
8. Algorithm comparison:
   - Autocomplete: Trigram+backoff vs. Bigram-only (100% vs 60% Recall@3)
   - Autocorrect: pyspellchecker vs. custom pure-Levenshtein correction (85% vs 55% accuracy)
9. Visualisation of autocorrect outcomes (corrected vs failed)
10. Discussion of limitations vs. production systems (Google Keyboard/Gboard)

## Folder naming for OIBSIP repo
Push this folder to your `OIBSIP` GitHub repo as:
`OIBSIP/DataAnalytics-L2-AutocompleteAutocorrect/`
