# Paumotu Linguistic Classifier: Modeling Tahitianization

## Abstract
This project applies Random Forest models to sociolinguistic fieldwork data from the Tuamotu Archipelago. It models "Tahitianization"—the phonological and lexical intrusion of high-prestige Tahitian on the native Paumotu substrate. By synthesizing phonetic glottalization rates and lexical loanword densities, the model identifies geographic patterns of language shift across five distinct atolls.

## The Data
The dataset consists of 25 linguistic samples across 5 speakers from **Ana'a, Fakarava, Apataki, Rangiroa, and Makatea**. 

**Key Features:**
* **Glottal_Rate:** Frequency of the intrusive /ʔ/ phoneme (Phonological shift).
* **Loanword_Rate:** Frequency of Tahitian lexical borrowings (Lexical shift).
* **Home_Atoll:** Geographic proxy for contact intensity.

## Methodology
I utilized a Random Forest Classifier to categorize samples into "High" vs. "Low" Tahitianization profiles. 
* **Architecture:** Ensemble of 200 Decision Trees.
* **Validation:** 70/30 Train-Test split with 3-fold Cross-Validation.
* **Performance:** The model achieved 100% Accuracy on the test set and a 95.8% Cross-Validation score, proving that glottal intrusion is a highly salient predictor of language shift.



## Key Findings
1.  **Phonological Dominance:** Feature importance analysis reveals that Glottal_Rate is a stronger predictor of Tahitianization than lexical borrowing.
2.  **Geographic Clustering:** Geographic hubs like Rangiroa and Fakarava exhibit significantly higher shift intensities compared to more conservative atolls like Ana'a.
3.  **Correlation:** A strong positive correlation exists between phonological and lexical intrusion, suggesting these shifts are synchronized within the speech community.



## Tech Stack
* **Language:** Python 3.9
* **Libraries:** Pandas, Scikit-learn, Matplotlib, Seaborn
* **Environment:** Jupyter Notebook
