# OilyGiant: Oil Well Selection and Profit Prediction Project

## 📌 Introduction

**OilyGiant** is planning a major investment in oil well development across three potential regions. This project aims to determine the most **profitable and low-risk region** using data-driven machine learning and statistical techniques.

We:

- Built a **Linear Regression** model to predict oil reserves for each region.
- Selected the **top 200 wells** in each region based on predicted reserves.
- Estimated the **expected profit** for each region using business constraints.
- Assessed the **risk of loss** using the **Bootstrapping technique**.
- Made a final **recommendation** on the best region for development.

---

## 💼 Business Constraints & Assumptions

- **Budget**: $100 million (cost to develop 200 wells).
- **Revenue per barrel**: $4.5K (reserves measured in 1000 barrels).
- **Only Linear Regression** models are permitted.
- **Regions analyzed**:
  - `geo_data_0`
  - `geo_data_1`
  - `geo_data_2`
- **Acceptable risk threshold**: Less than **2.5%** chance of loss.

---

## ⚙️ Methodology

1. **Data Preparation**:
   - Loaded and cleaned data for all three regions.
   - Merged geological features and product volumes.

2. **Modeling**:
   - Trained separate **Linear Regression** models for each region.
   - Predicted oil reserves on validation data.

3. **Profit Estimation**:
   - Selected top 200 predicted wells per region.
   - Calculated **expected profit** using:
     \[
     \text{Profit} = (\text{Predicted volume} \times 4500) - \text{Budget per well}
     \]

4. **Risk Analysis**:
   - Applied **bootstrapping** (1000 samples) on top 200 wells to estimate risk.
   - Evaluated probability of negative profit (loss).

---

## ✅ Results & Recommendation

After evaluating all three regions:

- **Region 1** showed:
  - 💰 **Highest average profit**: `$6.52 million`
  - 📉 **Near-zero risk of loss**

### ✅ **Region 1 is the optimal choice** for oil well development under the given constraints.

---

## 📦 Requirements

- Python 3.8+
- pandas
- numpy
- matplotlib / seaborn
- scikit-learn


📊 Future Improvements
Experiment with non-linear models (e.g., XGBoost or Random Forest).

Include geospatial analysis to better assess underground structure risks.

Consider multi-objective optimization for risk vs reward balance.

✍️ Author
Priti Sagar
Data Science Project | 2025

📄 License
This project is for educational purposes only.
No real financial or industrial decisions should be based on this analysis.





