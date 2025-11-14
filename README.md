# Divorce Prediction Analysis: A Study on Gottman's Couples Therapy Data

This project analyzes a dataset of 170 Turkish couples to identify the key statistical predictors of divorce. The analysis is based on the "Divorce Predictors Scale" (DPS) derived from Gottman's couples therapy principles.

- **See the full technical analysis:** [**divorce_analysis.ipynb**](analysis.ipynb)
- **See the summary presentation:** [**presentation/presentation.pdf**](presentation/presentation.pdf)

## Project Context

The dataset, sourced from Kaggle, contains responses to 54 questions from couples who were either "happily married" (Class 0) or "divorced" (Class 1). All responses were collected on a 5-point scale, where a higher score indicates a higher prevalence of problems.

The goal of this analysis was to move beyond individual questions and identify the *themes* that were most strongly correlated with divorce.

**Data Source:** [Gottman Divorce Predictors Dataset on Kaggle](https://www.kaggle.com/datasets/andrewmvd/divorce-predictors-data-based-on-gottman)

---

## Key Findings

The analysis revealed a clear distinction between two types of marital problems: **"Foundation Failures"** and **"Communication Breakdowns."**

While both are factors in divorce, their predictive power is dramatically different.

### 1. The Strongest Predictors: "Foundation Failures" (Corr: 0.89 - 0.94)

These 10 questions represent a fundamental misalignment in the relationship's core. They are the strongest statistical predictors of divorce. A high score on these indicates a lack of shared values, goals, and emotional harmony.

/presentation/graphs/most_influent_questions.png

### 2. The Weakest Predictors: "Communication Breakdowns" (Corr: 0.42 - 0.71)

This group of 10 questions perfectly describes the destructive communication patterns (Contempt, Defensiveness, Stonewalling) identified by Gottman.

/presentation/graphs/least_influent_questions.png

### The Big Idea:

While poor communication (like "The Four Horsemen") clearly erodes a marriage, **a lack of a shared foundation (values, dreams, roles) is the strongest predictor of divorce.**

This suggests that while communication can be repaired, a fundamental misalignment of values makes a stable marriage difficult to build from the start.

---

## Tech Stack

* **Python 3**
* **Pandas:** For data loading and manipulation.
* **Seaborn & Matplotlib:** For data visualization.
* **Jupyter Notebook:** For the analysis environment.

---

## How to Run This Project

1.  Clone this repository:
    ```bash
    git clone [https://github.com/peptesta/divorce_analysis.git](https://github.com/peptesta/divorce_analysis.git)
    ```
2.  If you want you can use the already downloaded dataset, or you can download it from the [Kaggle link](https://www.kaggle.com/datasets/andrewmvd/divorce-predictors-data-based-on-gottman).
3.  Place the `divorce_data.csv` and `reference.tsv` files into a `/data` folder (you may need to create this folder).
4.  Open `divorce_analysis.ipynb` in a Jupyter environment to view and run the full analysis.
