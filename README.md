# UK Road Accident Analysis

In this project we apply data cleaning, visualization, and machine-learning techniques to the publicly available **UK_Accident** dataset (over 1 M rows) from Kaggle:  
[Road Accident – United Kingdom Dataset](https://www.kaggle.com/datasets/devansodariya/road-accident-united-kingdom-uk-dataset)

We work on a **100 000-row sample** for rapid iteration, and also demonstrate a Spark pipeline on the full dataset.

---

## Repository Structure

```text
.
├── head.ipynb        # Pandas‐based EDA, preprocessing, ML & viz on 100 k rows
├── Spark.ipynb       # Apache Spark code on the full 1 M+ dataset
├── images/           # Generated visualizations
│   ├── 01_severity_histogram.png
│   ├── 02_accidents_by_day.png
│   ├── … etc.
└── README.md         # This file

```
For this project we selected the first 100,000 rows from the original dataset (with over 1,000,000 rows) to work with in `head.ipynb`.

`head.ipynb` contains code that works on the 100,000 row dataset. This dataset was preprocessed and feature engineered to suit machine learning & visualisation generation. Every stage of data preprocessing & visualisation saves a new file in working directory.

The `images` folder contains all 10 visualisation images generated from the partial 100,000 row datset.

The `Spark.ipynb` contains code that uses Apache Spark to evaluate the original big data dataset of over 1M entries. This code features no visualisations or saves any file when run.

The original dataset could not be uploaded on github due to its 25mb max upload limit. Get the original dataset from the link above, put in same working directory as `head.ipynb` and run. All other files will be automatically generated and saved in same working directory domino-effect style.

How to use

- Clone this repo
- Download and extract `UK_Accident.csv` into repo folder
- Run `head.ipynb`
- Run `Spark.ipynb`

This was a group work by 
- [Ferdinand Ekpo]
- [Radman Dhurbo]
- [Iliya Akila]
- [Ikpong Joseph](https://github.com/Ikpong-Joseph)

