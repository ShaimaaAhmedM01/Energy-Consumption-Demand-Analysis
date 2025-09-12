# 🔌 Energy Consumption & Demand Analysis  

## 📌 Overview  
This project analyzes household energy consumption data across regions and time, combining multiple datasets to explore usage patterns, test statistical hypotheses, and estimate cost-saving opportunities.  

The analysis uses **Python (Pandas, NumPy, Matplotlib, Seaborn, SciPy, Statsmodels)** for data cleaning, visualization, and hypothesis testing.  

---

## 📂 Dataset  
- **Sites Energy Consumption** (CSV – multiple parts merged)  
  - Columns: `DateTime`, `region`, `KWH/hh (per half hour)`  
- **Demand Data** (Excel)  
  - Columns: `DemandDateTime`, `Demand` (High, Normal, Low)  

---

## 🛠️ Steps  

### 1. Data Preparation  
- Combined 3 large CSV files into a single dataset.  
- Fixed datetime formats and aligned records to half-hour intervals.  
- Cleaned missing values and merged with demand data.  

### 2. Exploratory Data Analysis (EDA)  
- Distribution of energy consumption.  
- Energy usage by **region** (boxplots).  
- Consumption patterns by **hour of day** (line plots).  

### 3. Hypothesis Testing  
- **ANOVA** → Tested if regions differ in average energy consumption.  
- **Tukey’s post-hoc test** → Identified which regions significantly differ.  
- **Correlation** → Examined relationship between time of day and consumption.  

### 4. Business Insights  
- Defined a **low-consumption threshold** (25th percentile).  
- Estimated **potential savings (kWh + cost in EGP)** if usage is shifted.  

---

## 📊 Outputs  
- **Visualizations**: histograms, boxplots, line charts.  
- **Statistical Results**: ANOVA, Tukey test, correlations.  
- **Savings Estimates**: kWh reduction + cost savings in EGP.  
- Cleaned dataset: `Processed_Energy_Data.csv`.  

---

## 🚀 Tools Used  
- Python: `pandas`, `numpy`, `matplotlib`, `seaborn`  
- Statistics: `scipy`, `statsmodels`  
- Data: CSV + Excel (energy consumption & demand)  

---

## 🔑 Key Insights  
- Energy consumption varies significantly by **region**.  
- Strong correlation between **time of day** and usage.  
- Cost savings possible by shifting usage to **low-demand periods**.  

---
