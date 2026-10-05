# Titanic Dataset — Exploratory Data Analysis

An exploratory data analysis project using Python, Pandas, and Matplotlib to investigate survival patterns in the Titanic dataset.

## Objectives

- Load and inspect the Titanic dataset.
- Check missing values and data types.
- Analyze survival rates by sex and passenger class.
- Create age buckets and analyze survival across age groups.
- Visualize findings with bar charts, boxplots, and violin plots.
- Write a short insight report.

## Dataset

The dataset contains **891 passenger records and 12 original columns**.

Important columns:

| Column | Description |
|---|---|
| `Survived` | Survival status: 0 = No, 1 = Yes |
| `Pclass` | Passenger class |
| `Sex` | Passenger sex |
| `Age` | Passenger age |
| `Fare` | Ticket fare |
| `Embarked` | Port of embarkation |

### Missing values

The main missing values are:

- `Cabin`: 687
- `Age`: 177
- `Embarked`: 2

Age is left missing rather than artificially filling it for the age-group analysis.

## Age Groups

- Child: 0–12
- Teen: 13–18
- Young Adult: 19–35
- Adult: 36–60
- Senior: 61+

## Key Findings

1. Overall survival rate: **38.4%**.
2. Female survival rate: **74.2%** vs male: **18.9%**.
3. Class 1 had a **63.0%** survival rate, compared with **47.3%** for Class 2 and **24.2%** for Class 3.
4. The **Child (0–12)** group had the highest observed survival rate at **58.0%**.
5. Age-based results should be interpreted carefully because **177 Age values are missing**.

## Visualizations

- Survival rate by sex
- Survival rate by passenger class
- Survival rate by age group
- Age boxplot by survival status
- Age violin plot by survival status

## Technologies

- Python
- Pandas
- Matplotlib
- Jupyter Notebook

## Project Structure

```text
titanic-eda/
├── data/
│   └── Titanic-Dataset.csv
├── outputs/
│   ├── survival_by_sex.png
│   ├── survival_by_class.png
│   ├── survival_by_age_group.png
│   ├── age_boxplot_by_survival.png
│   └── age_violin_by_survival.png
├── analysis_results.txt
├── titanic_eda.ipynb
├── README.md
└── requirements.txt
```

## Learning Outcomes

This project helped me practice:

- Data loading and inspection
- Missing-value analysis
- Data type inspection
- Creating categorical features
- Group-by analysis
- Survival-rate calculation
- Data visualization
- Drawing insights from data

## Future Improvements

- Analyze survival using combinations such as sex + passenger class.
- Explore family size and fare.
- Perform more systematic missing-value treatment.
- Add further EDA and eventually build a machine learning model.

## Author

Oshin Gopal Thapa
