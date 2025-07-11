# 🏥 Medical Inventory Optimization Using Python

This project aims to streamline hospital inventory management by analyzing and optimizing medical supply data using Python. The dataset consists of over 14,000 records related to drug sales, returns, costs, and departmental usage. Through structured preprocessing and analysis, the goal is to uncover insights that support better stock decisions and reduce wastage.

## 📝 Project Highlights

- The dataset was first cleaned by identifying and removing:
  - Missing values in `DrugName`, `Formulation`, `SubCat`, and `SubCat1`
  - Duplicate rows (approximately 196 were removed)
- After cleaning, the data was reduced to 12,022 valid records.
- Numerical columns like `Final_Cost`, `Final_Sales`, `Quantity`, and `RtnMRP` were normalized using **MinMaxScaler** to prepare for further analysis and modeling.
- Feature selection using **VarianceThreshold** helped in identifying low-variance features which contributed little to predictive power.
- The `Final_Cost` was categorized into four ranges (bins) for better analysis: `0–25`, `25–50`, `50–75`, and `75–100`.

## 📊 Key Visual Insights

- Count plots revealed the distribution of `Sale` vs `Return` entries.
- Scatter plots between `Quantity` and `Final_Cost` highlighted cost-heavy drugs.
- Pie charts showed the proportion of sales per `Specialisation` and `Department`.
- Violin and box plots depicted cost/sales variations across departments and categories.
- Bar charts identified the top 10 most frequently dispensed drugs.

## ⚙️ Tools & Technologies Used

- **Python 3.10+**
- **Pandas** for data loading and preprocessing
- **Matplotlib** and **Seaborn** for visualization
- **Scikit-learn** for scaling and feature selection
- **Jupyter Notebook** for analysis and plotting

## 🎯 Goals of the Project

- Understand patterns in medical product sales and returns
- Optimize stock by identifying high-cost/low-usage drugs
- Enable hospital administrators to make data-driven decisions
- Prepare the data for future forecasting models or dashboards

## 🔮 Future Enhancements

- Integrate time series forecasting (ARIMA, LSTM) for stock demand prediction
- Deploy a real-time dashboard using **Streamlit** or **Dash**
- Link live hospital inventory systems for continuous data updates
- Extend the system to handle expiry tracking and reorder alerts

