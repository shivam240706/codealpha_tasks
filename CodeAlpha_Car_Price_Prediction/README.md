# 🚗 Task 3: Car Price Prediction 

## 📌 Project Goal
The objective of this project is to build a predictive Machine Learning regression model that accurately forecasts the secondary market selling price of used cars based on historical depreciation data, vehicle specifications, and original showroom prices.

**Data Source:** [Kaggle - Car Price Prediction Dataset](https://www.kaggle.com/datasets/vijayaadithyanvg/car-price-predictionused-cars)

---

## 📊 What Actually Drives a Car's Value?
Before modeling, we visually explored the data to understand the factors that dictate resale value:

### 1. The Biggest Clue: The Original Price
A mathematical correlation heatmap was generated to identify feature importance. 
* **Key Finding:** The original showroom price (`Present_Price`) is the absolute strongest predictor of a car's used price. 
* Additionally, newer cars hold their value well, while higher mileage slowly drops the overall price.

![Correlation Heatmap](images/correlation_heatmap.png)

### 2. Value Over Time (Depreciation)
By plotting the original price against the used selling price, we observe a clear trend line. Premium, high-end cars retain a significantly larger portion of their raw dollar value compared to budget-friendly vehicles.

![Scatter Plot](images/price_vs_original_scatter.png)

### 3. Fuel and Transmission Matter
Categorical analysis revealed that **Diesel** engines and **Automatic** transmissions usually command significantly higher resale prices than standard petrol or manual cars.

![Box Plot](images/fuel_type_boxplot.png)

---

## ⚙️ How We Built the Smart Model

### Preparing the Data for the Algorithm
Machine learning models require numeric matrices, so the dataset was meticulously preprocessed:
* **Categorical Encoding:** Text categories (like "Petrol" or "Automatic") were converted into binary numeric formats (1s and 0s) using One-Hot Encoding.
* **Noise Reduction:** The highly specific `Car_Name` column was dropped to prevent model overfitting and force the algorithm to focus on physical condition metrics rather than memorizing brand names.

### Model Performance
A **Multiple Linear Regression** algorithm was trained on the preprocessed dataset. 

* **Model Accuracy ($R^2$ Score):** **0.836**
* **Conclusion:** The model is highly accurate, successfully explaining 83.6% of the variance in real-world used car prices.

---

## 🌍 Real-World Business Applications
This machine learning logic powers massive businesses every day:
1. **Automated Dealership Pricing:** Platforms like CarMax or Carvana use similar regression models to instantly generate data-driven cash offers for customer vehicles.
2. **Insurance Valuation:** Insurance agencies rely on prediction algorithms to determine the exact payout value of a totaled vehicle based on current secondary market rates.
3. **Consumer Insights:** Valuation engines like Kelley Blue Book (KBB) utilize predictive modeling to give consumers fair-market estimates before negotiations.

---

## 💻 Tools Used
* **Python**
* **Scikit-Learn** (Machine Learning & Evaluation)
* **Pandas** (Data Preprocessing)
* **Seaborn & Matplotlib** (Visual EDA)

## 🚀 How to Run My Code
1. Ensure your `car_data.csv` is located in the `dataset/` folder.
2. Open your terminal and install the required libraries: `pip install -r requirements.txt`
3. Open the Jupyter Notebook and click **Restart & Run All**.