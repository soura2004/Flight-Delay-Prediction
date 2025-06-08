# Flight-Delay-Prediction

# ✈️ Flight Delay Analysis & Preprocessing (2016 U.S. Domestic Flights)

This project performs exploratory data analysis and preprocessing on a real-world U.S. domestic flight dataset from 2016. The primary goal is to prepare the data for a future machine learning model that can predict flight delays upon arrival (`ARR_DEL15`).

---

## 📂 Dataset Overview

- Source: U.S. Domestic Flight Data (2016)
- Total Rows: 11,231
- Columns: 26 (cleaned to 7 useful features for modeling)
- Target: `ARR_DEL15` (Binary: 0 = On time, 1 = Delayed over 15 minutes)

---

## 📊 Features Used

| Feature         | Description                              |
|----------------|------------------------------------------|
| `MONTH`         | Month of the flight                      |
| `DAY_OF_MONTH`  | Day of the month                         |
| `DAY_OF_WEEK`   | Day of the week (1 = Monday, ..., 7 = Sunday) |
| `ORIGIN`        | Origin airport code                      |
| `DEST`          | Destination airport code                 |
| `CRS_ARR_TIME`  | Scheduled arrival time (in HHMM format)  |
| `ARR_DEL15`     | Target label (0 = On time, 1 = Delayed)  |

---

## 🛠️ Workflow

### 1. **Data Loading & Exploration**
- Read CSV using `pandas`
- Inspected head, shape, and data types
- Identified null values

### 2. **Data Cleaning**
- Dropped irrelevant/unusable columns (e.g., `Unnamed: 25`)
- Focused only on columns relevant for modeling
- Verified and handled null values

### 3. **Feature Selection**
- Retained only features potentially useful for delay prediction

---

## 📉 Missing Data Summary

| Column       | Missing Entries |
|--------------|------------------|
| `ARR_DEL15`  | 188              |

Approach: These rows can either be dropped or imputed depending on modeling needs.

---

## 🔮 Next Steps

- Encode categorical features (e.g., `ORIGIN`, `DEST`)
- Feature engineering: time bins, traffic patterns, etc.
- Train ML models like Logistic Regression, Random Forest, or XGBoost
- Evaluate performance using accuracy, recall, precision, etc.

---

## 🧰 Tech Stack

- Python 3.x
- pandas
- numpy
- matplotlib & seaborn (for visualization)
- Jupyter Notebook

---

## 📁 Project Structure

📦 Flight-Delay-EDA
├── data/
│ └── FlightData.csv
├── flight_delay_analysis.ipynb
├── README.md

yaml
Copy
Edit


---

## 🧑‍💻 Author

**Sourajyoti Chakraborty**  
Feel free to reach out for questions or contributions!

---

## 📜 License

This project is open-source and available under the [MIT License](LICENSE).
