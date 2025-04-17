# 🐟 Fish Classification Project – STA2453

This repository contains the final project for STA2453 (Applied Statistics for Data Science), which aims to classify different species of Zooplankton based on the ecological features and various morphological features. The project includes exploratory data analysis (EDA), supervised learning models, evaluation metrics, and visualization.

## Project Objective

The goal of this project is to build a robust classifier that predicts the species of Zooplankton using features such as length, weight, height, and width. Multiple machine learning models are compared to assess classification performance, including:

- Logistic Regression
- Random Forest
- XGBoost

This project demonstrates the full data science workflow, from data cleaning to model evaluation and final visualization.

---

## Project Structure

```bash
├── data/               # Cleaned datasets to be saved in EDA
├── EDA/                # Jupyter notebooks for data preprocessing, EDA and Visualization
├── Modelling/          # Output figures, confusion matrices, and evaluation tables
├── requirements.txt    # List of required Python packages
```

## How to Reproduce the Work

1. Clone the Repository

```bash
git clone https://github.com/DaihaoWu/STA2453.git
cd STA2453
```

2. Set Up a Virtual Environment
   We recommend using venv or conda:

Using venv:

```bash
python3 -m venv fishenv
source fishenv/bin/activate  # On Windows: fishenv\Scripts\activate
pip install -r requirements.txt
```

Using conda:

```bash
conda create -n fishenv python=3.9
conda activate fishenv
pip install -r requirements.txt
```

## Results Summary

After model evaluation, the Random Forest classifier achieved the best performance with:

📬 Contact
For questions or collaboration, feel free to reach out at daihao.wu@mail.utoronto.ca
