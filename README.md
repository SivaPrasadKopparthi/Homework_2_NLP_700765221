# Homework 2 – CS5760 Natural Language Processing

**Student Name:** Sai Siva Shankara Vara Prasad Kopparthi

**Student ID:** 700765221

**Course:** CS5760 Natural Language Processing – Fall 2025

**University:** University of Central Missouri

---

## 📌 Overview

This repository contains my solutions for **Homework 2** of CS5760 NLP.
The assignment demonstrates key NLP concepts, including **Bayesian classification, smoothing, evaluation metrics, probabilistic language models, and backoff modeling**.

The repository includes:

* **Detailed written answers (Q1–Q8)**.
* **Jupyter Notebook (`Homework 2.ipynb`)** that contains Python implementations for Q5 (evaluation metrics) and Q8 (bigram language model).
* Explanations, reasoning, and interpretations for all tasks.

---

## 📝 Questions and Answers Summary

### Q1 – Bayes’ Rule Applied to Text

* Defined prior, likelihood, posterior, and evidence in the context of document classification.
* Explained why the denominator **P(d)** can be ignored when comparing classes.
* Demonstrates the foundation of Naive Bayes text classification.

### Q2 – Add-1 Smoothing

* Applied Laplace smoothing to handle sparse data.
* Computed denominators for the negative class (34) and estimated probabilities for words like *predictable* and *fun*.
* Highlighted how smoothing prevents zero probabilities for unseen words.

### Q3 – Worked Example Classification

* Classified the document *“predictable no fun”* step by step.
* Computed probabilities for both positive and negative classes.
* Final result: **Positive class**, since its score is higher.

### Q4 – Harms of Classification

* Explained **representational harm** using the Kiritchenko & Mohammad (2018) study.
* Discussed risks of **censorship in toxicity classification**.
* Noted that models may underperform on AAE or Indian English due to lack of training data.
* Emphasized fairness issues in real-world NLP systems.

### Q5 – Evaluation Metrics

* Calculated **precision and recall** per class (Cat, Dog, Rabbit).
* Compared **macro-averaged** and **micro-averaged** metrics.
* Explained how macro emphasizes fairness across classes, while micro reflects overall accuracy.
* ✅ Implemented in **Homework 2.ipynb** with automated calculations and results.

### Q6 – Bigram Probabilities & Zero-Probability Problem

* Compared probabilities of two sentences using a bigram model.
* Found **S1 (<s> I love NLP </s>)** more probable.
* Illustrated the **zero-probability problem** when unseen words like “noodle” occur.
* Applied Laplace smoothing to assign small nonzero probabilities.

### Q7 – Backoff Model

* Computed trigram and backed-off bigram probabilities for given contexts.
* Showed how **backoff handles unseen trigrams**.
* Explained why backoff is essential to avoid zero-probability issues in sparse corpora.

### Q8 – Bigram Language Model Implementation

* Implemented a bigram language model in **Homework 2.ipynb**.
* Calculated unigram/bigram counts and probabilities.
* Compared sentence probabilities for *S1* and *S2*, showing the model prefers **S1**.
* Demonstrated how statistical language models naturally favor sequences better supported by training data.

---

## 💻 Code

All programming tasks (Q5 & Q8) are implemented in:

* **`Homework 2.ipynb`** → Jupyter Notebook containing Python code, calculations, and outputs.
