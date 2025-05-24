# SpamLyte: Lightweight Stacking Approach for Spam Detection  
**Final Year Project - Lua Chong En [20417309]**

---

## Project Overview
**SpamLyte** : Lightweight Stacking Approach for Spam Detection

Notebook Environment: **Jupyter Notebook (Google Colab)**

---

## Pre-requisites

Before running this notebook on Google Colab, ensure the following:

1. Upload all original dataset files (e.g., `n.xlsx`, ranging from 4,000 to 16,000 samples).
2. Upload all TF-IDF feature extracted files (e.g., `tfidf_file1000-n.xlsx`). - This is pre-processed, so it can be fed into the models directly.
3. Dataset can also be downloaded from [Kaggle](https://kaggle.com/datasets/5cc5fc5934ccd6336b7ef938834d5038ad795ad66927783caceea6ad529cddad).
4. Ensure all files are uploaded to Colab **before** running any notebook cell.

---

## Contents

This notebook is split into 12 sections - Use the table to contents to navigate to each section

1.Forcefully install nltk version 3.8.1 due to ongoing dependency problem
2.Data Pre-processing
3.Support Vector Machine (Classifier)
4.Random Forest (Classifier)
5.Multinomial Naive Bayes (Classifier)
6.K-Nearest-Neighbors (Classifier)
7.Logistic Regression (Meta-model)
8.Stacking (MNB, SVM, DT) + (LR) - Combination 1
9.Stacking (MNB, KNN, DT) + (LR) - Combination 2
10.Stacking (MNB, Perceptron, DT) + (LR) - Combination 3
11.Stacking (MNB, LightGBM, RF) + (LR) - Combination 4
12.Final Stacking Technique (MNB, KNN, RF) + (LR) - Combination 5

---

## Instructions

To run this project:

1. Open the notebook in [Google Colab](https://colab.research.google.com).
2. At the top menu, select:  
   `Runtime` -> `Change runtime type` -> Set **Hardware accelerator** to `CPU`.
   Or at the top right corner, select:
   `Connect` -> It will automatically connect to Google Python 3 backend using CPU
3. Force install the correct `nltk` version due to dependency issues:
   ```python
   !pip install nltk==3.8.1 --force-reinstall
