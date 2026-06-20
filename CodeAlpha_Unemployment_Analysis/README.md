# Unemployment Analysis in India (Covid-19 Impact)

## Project Overview
This is a beginner-friendly data science project that looks at how the strict Covid-19 lockdowns in 2020 affected the job market in India.

**Data Source:** [Kaggle - Unemployment in India Dataset](https://www.kaggle.com/datasets/gokulrajkmv/unemployment-in-india)

## What I Did in This Project
* **Data Cleaning:** Fixed missing values and date formats so the math and graphs would work perfectly.
* **Data Visualization:** Made different charts to clearly see the trends, like how the unemployment rate spiked exactly during the lockdown months.
* **Adding New Features:** Created a new "Severity" column to easily label which areas had "High" or "Low" unemployment compared to the rest of the country.
* **Before vs. After:** Compared the 2020 pandemic data to normal, pre-covid years to prove exactly how much the lockdowns hurt the job market.

## 📊 Visualization Highlights
Here are the key patterns found during the analysis:

**1. Distribution of Unemployment Rates**
![Unemployment Distribution](images/unemployment_distribution.png)

**2. Covid-19 Impact Trend**
![Covid Impact](images/covid_timeline.png)

**3. Average Unemployment by State**
![State Analysis](images/state_analysis.png)

**4. Correlation Heatmap**
![Correlation](images/correlation_heatmap.png)

## Tools I Used
* Python
* Pandas & NumPy (for data cleaning and math)
* Matplotlib & Seaborn (for drawing the graphs)
* Jupyter Notebook

## Final Conclusion
Even though the overall yearly average for 2020 only went up a little bit, the line graphs show the real story. There was a massive, sudden shock during the strict lockdown months, causing the unemployment rate in the worst-hit states to temporarily spike all the way to 75.85%.

## How to Run My Code
1. Download or clone this folder to your computer.
2. Open your terminal and install the required tools by typing: `pip install -r requirements.txt`
3. Open `Unemployment_Analysis.ipynb` in Jupyter Notebook and run the cells from top to bottom.