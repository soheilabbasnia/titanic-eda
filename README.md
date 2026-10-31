# Titanic Exploratory Data Analysis (EDA)

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)
[![Python: 3.x](https://img.shields.io/badge/Python-3.x-3776AB.svg?logo=python&logoColor=white)](https://python.org)
[![Jupyter](https://img.shields.io/badge/Notebook-Jupyter-F37626.svg?logo=jupyter&logoColor=white)](https://jupyter.org)
[![Dataset: Kaggle](https://img.shields.io/badge/Dataset-Kaggle%20Titanic-20BEFF.svg?logo=kaggle&logoColor=white)](https://www.kaggle.com/c/titanic)

English | [فارسی](README_FA.md)

A comprehensive data cleaning, statistical investigation, and **Exploratory Data Analysis (EDA)** project on the historic Kaggle Titanic passenger dataset, uncovering socio-demographic factors influencing survival rates during the 1912 maritime disaster.

---

## 🌟 Overview

On April 15, 1912, the RMS Titanic collided with an iceberg during her maiden voyage and sank, resulting in the loss of over 1,500 lives out of 2,224 passengers and crew.

This repository provides an in-depth data exploration workflow utilizing **Python**, **Pandas**, **NumPy**, **Matplotlib**, and **Seaborn**. The project emphasizes disciplined data preprocessing, missing data strategies, bivariate correlations, and statistical visualizations to answer fundamental demographic questions surrounding passenger survival.

Key highlights:
- **Systematic Cleaning Pipeline**: Methodical assessment and handling of missing values in `Age`, `Cabin`, and `Embarked`.
- **Feature Relationships & Correlation**: In-depth analysis of passenger class (`Pclass`), gender (`Sex`), fare distribution, and family presence (`SibSp` + `Parch`).
- **Visual Storytelling**: High-resolution distribution plots, heatmaps, box plots, and survival proportion charts.
- **Reproducible Analysis**: Executable Jupyter Notebook (`eda.ipynb`) with step-by-step documentation and commentary.

---

## 📊 Dataset Dictionary

The dataset contains records for 891 individual passengers with 12 attributes:

| Column | Description | Key Values / Range |
| :--- | :--- | :--- |
| `PassengerId` | Unique sequential identifier for each passenger | 1 to 891 |
| `Survived` | Survival indicator | `0` = No, `1` = Yes |
| `Pclass` | Passenger ticket class | `1` = 1st (Upper), `2` = 2nd (Middle), `3` = 3rd (Lower) |
| `Name` | Full name of the passenger | String |
| `Sex` | Biological sex | `male`, `female` |
| `Age` | Age in years (fractional if `<1`) | 0.42 to 80.0 |
| `SibSp` | Number of siblings or spouses aboard | 0 to 8 |
| `Parch` | Number of parents or children aboard | 0 to 6 |
| `Ticket` | Ticket number string | Alphanumeric |
| `Fare` | Passenger fare paid | \$0.00 to \$512.33 |
| `Cabin` | Cabin number | Alphanumeric (sparse) |
| `Embarked` | Port of embarkation | `C` = Cherbourg, `Q` = Queenstown, `S` = Southampton |

---

## 💡 Key Analysis Findings

1. **Gender Disparity ("Women and Children First")**: Female passengers had an overwhelmingly higher survival rate (~74%) compared to male passengers (~19%).
2. **Socio-Economic Privilege (Class Divide)**: 1st class passengers had a survival rate exceeding 62%, whereas 3rd class passengers had a survival rate below 25%.
3. **Family Dynamics**: Passengers traveling with small families (1–3 members) exhibited higher survival probabilities than solo travelers or individuals with large families (5+).
4. **Age Distribution**: Young children had prioritized lifeboat access, while elderly passengers experienced significantly lower survival rates.

---

## 🚀 Getting Started

### Prerequisites

- Python 3.8 or higher
- Jupyter Notebook or JupyterLab

### Installation & Execution

1. **Clone the repository**:
   ```bash
   git clone https://github.com/soheilabbasnia/titanic-eda.git
   cd titanic-eda
   ```

2. **Create and activate a virtual environment**:
   ```bash
   python3 -m venv .venv
   source .venv/bin/activate
   ```

3. **Install dependencies**:
   ```bash
   pip install pandas numpy matplotlib seaborn jupyter
   ```

4. **Launch the analysis notebook**:
   ```bash
   jupyter notebook eda.ipynb
   ```

---

## 📁 Project Structure

```text
titanic-eda/
├── titanic.csv             # Kaggle Titanic passenger dataset (891 rows)
├── eda.ipynb               # Full Jupyter Notebook with analysis & plots
├── LICENSE                 # MIT License
└── README.md               # English project documentation
```

---

## 🤝 Contributing

Contributions, feedback, and additional feature engineering analyses are welcome!
1. Fork the repository.
2. Create your feature branch (`git checkout -b feature/model-prediction`).
3. Commit your changes (`git commit -m 'Add logistic regression model'`).
4. Push to the branch (`git push origin feature/model-prediction`).
5. Open a Pull Request.

---

## 📜 License

This project is licensed under the [MIT License](LICENSE).
Open source for educational, research, and non-commercial purposes.
