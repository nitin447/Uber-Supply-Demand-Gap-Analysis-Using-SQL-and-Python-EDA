# 🚖 Uber Supply–Demand Gap Analysis

This project analyzes Uber ride request data to identify the gap between **customer demand** and **driver supply**.  
Using **SQL** for data extraction and **Python** for data cleaning, exploratory data analysis (EDA), and visualization, the project uncovers key patterns affecting ride availability and cancellation rates.

---

## 📌 Project Overview
- **Goal:** Understand why and when Uber faces supply shortages compared to ride demand.
- **Approach:** Extract trip data using SQL, clean and analyze it using Python, and visualize patterns for better decision-making.
- **Outcome:** Insights to optimize driver allocation and improve customer satisfaction.

---

## 🛠 Tech Stack
- **Languages:** SQL, Python
- **Libraries:** Pandas, NumPy, Matplotlib, Seaborn
- **Tools:** Jupyter Notebook / Google Colab, MySQL / SQLite

---

## 📊 Analysis & Insights

### 1. Data Extraction (SQL)
- Queried the raw trip request data from the database.
- Filtered out incomplete entries and irrelevant columns to focus on demand–supply metrics.
- Used `GROUP BY` and `JOIN` operations to segment data by pickup point, time, and trip status.

### 2. Data Cleaning (Python)
- Converted timestamp columns to `datetime` format for time-based analysis.
- Removed duplicates and handled missing values in critical columns.
- Standardized categorical variables (e.g., "No Cars Available", "Cancelled").

### 3. Exploratory Data Analysis (EDA)
- **Demand vs Supply Trends:**  
  Found a significant mismatch during **morning airport pickups (5 AM–9 AM)** and **evening city pickups (5 PM–9 PM)**.
- **Cancellation Hotspots:**  
  High trip cancellations during peak hours, especially from city pickups to airport destinations.
- **Driver Availability:**  
  Shortage of drivers is the main reason for the supply–demand gap, not high cancellations by drivers.

### 4. Visual Insights
- **Bar Charts:** Showed hourly ride requests vs rides fulfilled.
- **Heatmaps:** Highlighted locations and times with the highest shortage.
- **Line Graphs:** Depicted cancellation rate fluctuations across different times of the day.

### 5. Key Findings
- Peak demand periods consistently show a shortfall in available drivers.
- Early morning airport requests often go unfulfilled due to driver shortage.
- Evening city pickup shortages cause increased customer wait times and cancellations.

### 6. Recommendations
- Increase driver deployment in high-demand zones during identified peak hours.
- Offer incentives for drivers to accept trips during early morning and late evening.
- Use historical data to implement predictive driver allocation strategies.

1. **Clone the Repository**
   ```bash
   git clone https://github.com/your-username/uber-supply-demand-gap.git
   cd uber-supply-demand-gap
