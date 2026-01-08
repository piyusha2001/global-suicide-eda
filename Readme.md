# Global Suicide EDA & Statistical Analysis

This project performs a rigorous exploratory and statistical analysis of global suicide data sourced from the World Health Organization (WHO). The goal is to uncover multivariate relationships between demographics, economic factors, and suicide rates, validated through inferential statistics.

https://github.com/user-attachments/assets/71da4366-293b-4bf5-abd6-c7f75e3ec9fa

## 🧪 Project Overview

Beyond standard visualization, this project applies mathematical modelling to validate trends:
1.  **Data Cleaning & Preprocessing:** Handling missing values, standardizing country names, and outlier detection.
2.  **Exploratory Data Analysis (EDA):** Visualizing distributions across age groups, genders, and timelines.
3.  **Inferential Statistics:** Using **SciPy** to perform hypothesis testing and correlation analysis.

## 📊 Statistical Methodologies

The `main.ipynb` notebook includes specific statistical verifications:

### 1. Hypothesis Testing (T-Test)
*   **Objective:** To determine if the difference in suicide rates between male and female demographics is statistically significant or due to random chance.
*   **Method:** Applied `scipy.stats.ttest_ind` (Independent T-test).
*   **Result:** The analysis yielded a **p-value < 0.05**, rejecting the null hypothesis and statistically confirming significant gender disparities in suicide rates.

### 2. Multivariate Analysis (Pearson Correlation)
*   **Objective:** To quantify the linear relationship between numerical variables (Population, Year, Suicide Count).
*   **Method:** Calculated the **Pearson Correlation Coefficient** matrix and visualized it via a Seaborn heatmap.
*   **Result:** identified a moderate-to-strong positive correlation (**0.61**) between population size and total suicide incidents.

## 📂 Project Structure

- **`data/who_suicide_statistics.csv`**: Raw dataset containing Country, Year, Age Group, Gender, Population, and Suicide counts.
- **`notebooks/main.ipynb`**: The core analysis notebook containing data cleaning, visualizations, and statistical code blocks.
- **`outputs/`**: Generated visualizations and processed data.

## 🛠️ Technologies Used

- **Python 3.x**
- **Pandas & NumPy:** Data manipulation and vectorization.
- **SciPy:** Statistical functions (T-tests, P-value calculation).
- **Seaborn & Matplotlib:** Data visualization and heatmaps.

## License

This project is licensed under the MIT License. See the `LICENSE` file for details.

## Acknowledgments

- World Health Organization (WHO) for the raw dataset.
