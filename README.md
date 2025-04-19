# 🐟 Fish Classification Project – STA2453

This repository contains the final project for STA2453 (Applied Statistics for Data Science), which aims to classify different species of Zooplankton based on the ecological features and various morphological features. The project includes exploratory data analysis (EDA), supervised learning models, evaluation metrics, and visualization.

## Project Objective

The goal of this project is to build a robust classifier that predicts the species of Zooplankton using features such as length, weight, height, and width. Multiple machine learning models are compared to assess classification performance, including:

- Logistic Regression
- Random Forest
- XGBoost

This project demonstrates the full data science workflow, from data cleaning to model evaluation and final visualization.

For more details, check out the final report on the project : [Final_Report.pdf](/STA2453/Zooplankton_Final_Report.pdf)

---

## Project Structure

```bash
├── EDA/                # Jupyter notebooks for data preprocessing, EDA and Visualization
├── Modelling/          # Output figures, confusion matrices, and evaluation tables
├── requirements.txt    # List of required Python packages
```

### EDA

The [EDA](/STA2453/EDA/) folder contains the complete exploratory data analysis workflow for the project. It includes code for data preprocessing and cleaning, merging the geometric and environmental datasets, performing descriptive analysis, and generating key visualizations. This step serves as the foundation for understanding data quality, feature distributions, class imbalances, and correlations—providing essential insights to guide the subsequent modeling phase.

### Modelling

The [Modelling](/STA2453/Modelling/) folder contains multiple juptor notebook file that shows the code and the results for multiple attempt in different modelling methods. The [Random_Forest](/STA2453/Modelling/Random_Forest.ipynb) notebook contains the code for modelling with solely the 7 target class, while the other random forest notebook contains the modelling approach for all classes.

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

After model evaluation, the XGBoost classifier achieved the best performance with:

| Model                 | Accuracy (%) | Macro F1 (%) | Weighted F1 (%) |
| --------------------- | ------------ | ------------ | --------------- |
| Logistic Regression   | 81.7         | 53.9         | 79.9            |
| Random Forest (SMOTE) | 86.0         | 67.0         | 87.0            |
| XGBoost (SMOTE)       | **89.2**     | **68.4**     | **88.7**        |

## Contact

For questions or collaboration, feel free to reach out at daihao.wu@mail.utoronto.ca
