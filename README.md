# EDA
Task 5 of Elevate labs
# Exploratory Data Analysis (EDA) on Titanic Dataset

This project involves performing basic exploratory data analysis (EDA) on the Titanic dataset to understand the structure, clean the data, and visualize important patterns.

---

## 1. Initial Data Exploration

- **Dataset Shape:** 891 rows × 12 columns
- **Key Variables:** 
  - Numerical: Age, Fare, SibSp, Parch
  - Categorical: Pclass, Sex, Embarked
- **Missing Values:** 
  - Age: 177 missing
  - Cabin: 687 missing
  - Embarked: 2 missing

### Actions Taken:
- Imputed missing `Age` values with median per `Pclass`.
- Created a binary `Has_Cabin` feature indicating presence of cabin information.
- Filled missing `Embarked` values with the mode.
- Extracted `Title` from the `Name` field.
- Created a `Family_Size` feature as `SibSp + Parch`.

---

## 2. Data Visualization

### a. Pairplot for Numerical Variables
- Visualized relationships between variables like Age, Fare, SibSp, Parch with Survival as the hue.

### b. Correlation Heatmap
- Created a heatmap showing correlation between numerical features.

### c. Survival by Passenger Class
- Compared survival counts across different passenger classes.

### d. Age Distribution by Survival
- Plotted the age distribution for survived vs non-survived passengers.

### e. Survival by Sex
- Compared survival counts across genders.

---

## Libraries Used
- pandas
- numpy
- seaborn
- matplotlib

---

## How to Run
```bash
# Clone the repository
git clone https://github.com/Gauri2882/EDA

# Install required libraries
pip install pandas numpy matplotlib seaborn

# Run the Jupyter Notebook
