# Carbon Emission Dataset Analysis

## Project Overview
This project presents an exploratory data analysis of the **Carbon Emission Dataset** using Python.  
The work was completed as part of the *Advanced Python Project* for the second semester of 2025/2026.

The main objective is to clean the dataset, explore the most important variables, create visualizations,
study relationships between features, and analyze time‑based behavior of carbon emissions using
Pandas, NumPy, Matplotlib, and Seaborn.

## Dataset
The dataset used in this project is **`carbon_emission_dataset_with_Industry.csv`**.  
It contains daily company‑level records that combine operational, financial, and environmental
indicators, such as:

- Energy consumption (total, renewable, non‑renewable)
- Production output
- Supply chain transport distance
- Raw material usage
- Carbon tax and energy cost
- Expected renewable share and expected carbon reduction
- Industry sectors and social impact indicators
- Target variable: **`Carbon_Emission_tCO2e_TARGET`**

## Tools and Libraries
The analysis was implemented using:

- Python 3
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Statsmodels (for time‑series decomposition)

## Project Tasks
This project covers the required assignment tasks:

1. **Load and inspect data**
   - Import the dataset, view the first rows, check `info()` and `describe()`.

2. **Data cleaning**
   - Handle missing values.
   - Remove duplicate rows.
   - Convert the `Date` column to datetime.
   - Ensure numeric and categorical data types are correct.

3. **Exploratory (Univariate) analysis**
   - Compute mean, median, min, and max for:
     `Total_Energy_Consumption_kWh`,
     `Renewable_Energy_Consumption_kWh`,
     `NonRenewable_Energy_Consumption_kWh`,
     `Production_Output_Units`,
     `Supply_Chain_Transport_km`.
   - Plot distributions (histograms + KDE) and frequency bar charts.
   - Plot energy variables over time.

4. **Bivariate & multivariate analysis**
   - Scatter plots between key energy variables and emissions.
   - Correlation heatmap for numerical variables.
   - Box plot of `Carbon_Emission_tCO2e_TARGET` by `Industry_Sectors`.
   - Pairplot for selected features.
   - Grouped analysis of emissions by industry sector.

5. **Time‑series analysis**
   - Plot emissions over time.
   - Plot rolling mean and rolling variance.
   - Apply time‑series decomposition (trend and seasonality).

6. **Analytical questions (Q1–Q5)**
   - Identify emission sources with highest variability.
   - Check whether emissions are normally distributed.
   - Find variables most strongly correlated with emissions.
   - Discuss the presence of a trend in emissions.
   - Discuss possible seasonal patterns.

## Main Findings
- Energy‑related variables, especially **total** and **non‑renewable** energy consumption,
  show the highest variability in the dataset.
- Carbon emissions are strongly positively correlated with:
  - `NonRenewable_Energy_Consumption_kWh`
  - `Carbon_Tax_USD`
  - `Total_Energy_Consumption_kWh`
- `Expected_Renewable_Share_Percent` is negatively correlated with emissions, suggesting
  that higher expected renewable share is associated with lower carbon emissions.
- The distribution of `Carbon_Emission_tCO2e_TARGET` is skewed and does **not** follow a
  perfect normal distribution.
- Time‑series plots and rolling statistics reveal structured temporal behavior rather than
  purely random fluctuations.

## Files Included
Typical repository contents:

- `carbon_emission_required_only.ipynb` – main notebook with code and figures.
- `carbon_emission_report.pdf` – final report summarizing the analysis.
- `carbon_emission_dataset_with_Industry.csv` – dataset (if allowed to include).
- `README.md` – this project description.

## How to Run
1. Open the notebook in **Google Colab** or **Jupyter Notebook**.
2. Upload `carbon_emission_dataset_with_Industry.csv` to the notebook environment.
3. Update the file path if necessary.
4. Run all cells from top to bottom.
5. Review the output tables, charts, and the answers to Q1–Q5.

## Course Information
- **Course:** Advanced Python Project  
- **Semester:** Second Semester 2025/2026  
- **Instructors:** Dr. Ali Azwai and Dr. Ala Abuthawabeh  

## Author
**Student:** Mohamed Alramamneh
