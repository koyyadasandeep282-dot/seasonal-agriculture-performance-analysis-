# 🌾 Seasonal Agriculture Performance Analysis

## 📌 Project Overview

**Seasonal Agriculture Performance Analysis** is a Python-based data analysis project that studies agricultural performance across different **seasons, crops, states, irrigation methods, environmental conditions, production factors, water usage, and financial outcomes**.

The project uses Python data-analysis and visualization libraries to clean, analyze, and visualize a dataset containing **4,000 farm records and 28 attributes**.

The main objective is to identify patterns and relationships between agricultural conditions and important outcomes such as **crop yield, production, revenue, profit, water efficiency, and disease/pest risk**.

---

## 🎯 Objectives

* Analyze agricultural performance across different seasons.
* Compare crop-wise and state-wise performance.
* Study the relationship between environmental factors and crop yield.
* Analyze irrigation methods and their relationship with yield.
* Evaluate water usage and water efficiency.
* Analyze revenue, production costs, and profit.
* Identify correlations between agricultural variables.
* Detect missing values and duplicate records.
* Generate meaningful visualizations and summary reports.
* Extract key findings that can support agricultural analysis and planning.

---

## 📊 Dataset

The dataset contains **4,000 records and 28 columns**.

### Dataset Features

| Feature                         | Description                       |
| ------------------------------- | --------------------------------- |
| `Farm_ID`                       | Unique farm identifier            |
| `State`                         | State where the farm is located   |
| `District`                      | District associated with the farm |
| `Crop`                          | Crop cultivated                   |
| `Season`                        | Agricultural season               |
| `Farm_Area_Hectares`            | Farm area in hectares             |
| `Rainfall_mm`                   | Rainfall received                 |
| `Avg_Temperature_C`             | Average temperature               |
| `Humidity_pct`                  | Humidity percentage               |
| `Sunlight_Hours_Day`            | Daily sunlight hours              |
| `Soil_pH`                       | Soil pH level                     |
| `Soil_Moisture_pct`             | Soil moisture percentage          |
| `Nitrogen_kg_ha`                | Nitrogen quantity                 |
| `Phosphorus_kg_ha`              | Phosphorus quantity               |
| `Potassium_kg_ha`               | Potassium quantity                |
| `Irrigation_Method`             | Irrigation technique used         |
| `Fertilizer_kg_ha`              | Fertilizer usage                  |
| `Pesticide_Litre_ha`            | Pesticide usage                   |
| `Seed_Quality_Score`            | Seed quality score                |
| `Yield_Tonnes_Ha`               | Yield per hectare                 |
| `Production_Tonnes`             | Total production                  |
| `Market_Price_INR_Tonne`        | Market price per tonne            |
| `Total_Cost_INR`                | Total production cost             |
| `Revenue_INR`                   | Revenue generated                 |
| `Profit_INR`                    | Profit or loss                    |
| `Water_Used_m3`                 | Water consumption                 |
| `Water_Efficiency_t_per_1000m3` | Water efficiency                  |
| `Disease_Pest_Risk_pct`         | Disease/pest risk percentage      |

The dataset contains three seasons: **Kharif, Rabi, and Zaid**, eight crops, eight states, and four irrigation methods.

---

## 🛠️ Technologies Used

* **Python**
* **NumPy**
* **Pandas**
* **Matplotlib**
* **Seaborn**
* **Google Colab / Jupyter Notebook**
* **CSV Dataset**

The project imports Pandas, NumPy, Matplotlib, and Seaborn for data processing and visualization.

---

## 🔄 Project Workflow

```text
Dataset
   ↓
Load Data
   ↓
Data Exploration
   ↓
Data Cleaning
   ↓
Missing Value Handling
   ↓
Duplicate Detection
   ↓
Exploratory Data Analysis
   ↓
Statistical Analysis
   ↓
Data Visualization
   ↓
Correlation Analysis
   ↓
Performance Comparison
   ↓
Key Findings
   ↓
CSV Summary Reports
```

---

## 🧹 Data Cleaning

The project checks for:

* Missing values
* Missing-value percentages
* Duplicate records
* Data types
* Dataset dimensions
* Unique categorical values

Missing values in the following numerical columns are handled using the **median**:

* `Rainfall_mm`
* `Soil_Moisture_pct`
* `Yield_Tonnes_Ha`

The project then checks the dataset again to confirm that missing values have been handled.

The original dataset contained:

* 48 missing rainfall values
* 40 missing soil-moisture values
* 32 missing yield values

## After cleaning, no missing values remained, and no duplicate records were found.

## 📈 Analysis Performed

### 1. Seasonal Analysis

The project calculates and visualizes:

* Number of farms by season
* Average yield by season
* Yield distribution
* Average production
* Average profit
* Revenue, cost, and profit
* Water usage
* Disease/pest risk
* Rainfall
* Temperature

The analysis compares **Kharif, Rabi, and Zaid** seasons.

### 2. Crop-Wise Analysis

The project evaluates each crop based on:

* Average yield
* Average production
* Average profit
* Water efficiency

The dataset contains:

* Wheat
* Maize
* Pulses
* Rice
* Cotton
* Chilli
* Groundnut
* Sugarcane

### 3. State-Wise Analysis

Agricultural performance is compared across:

* Andhra Pradesh
* Maharashtra
* Telangana
* Karnataka
* Gujarat
* Tamil Nadu
* Punjab
* Madhya Pradesh

The analysis measures average yield, production, and profit by state.

### 4. Irrigation Analysis

Four irrigation methods are analyzed:

* Drip
* Flood
* Rainfed
* Sprinkler

The project compares their usage and average crop yield.

### 5. Environmental Analysis

The project studies relationships between:

* Rainfall and yield
* Temperature and yield
* Fertilizer usage and yield
* Seasonal conditions and yield

Scatter plots are used to visualize these relationships.

### 6. Financial Analysis

The project examines:

* Revenue
* Total cost
* Profit
* Production
* Yield

It also studies relationships such as:

* Yield vs Profit
* Production vs Profit
* Revenue vs Profit

### 7. Correlation Analysis

A correlation matrix is generated for numerical variables to examine relationships among agricultural, environmental, production, and financial variables.

A correlation heatmap is also created using Seaborn.

---

## 📊 Visualizations

The project generates several visualizations, including:

* Season-wise farm count
* Average yield by season
* Yield distribution by season
* Average production by season
* Average profit by season
* Revenue vs cost vs profit
* Average profit by crop
* Average yield by crop
* Average profit by state
* Water usage by season
* Water efficiency by crop
* Disease/pest risk by season
* Rainfall distribution
* Temperature distribution
* Irrigation-method distribution
* Yield by irrigation method
* Fertilizer vs yield
* Rainfall vs yield
* Temperature vs yield
* Yield vs profit
* Production vs profit
* Revenue vs profit
* Correlation heatmap
* Profit and yield outlier plots

---

## 🔍 Key Findings

According to the analysis:

### Seasonal Performance

Average yield:

| Season | Average Yield (Tonnes/Ha) | Average Profit (INR) |
| ------ | ------------------------: | -------------------: |
| Kharif |                      5.63 |          ₹178,914.65 |
| Rabi   |                      5.04 |           ₹87,689.47 |
| Zaid   |                      4.64 |          -₹24,804.82 |

Kharif has the highest average yield and profit among the three seasons in this dataset. Zaid has a negative average profit.

### Crop Performance

Sugarcane has the highest average profit and average yield in the crop-wise analysis:

* Average yield: **46.64 tonnes/ha**
* Average production: **392.41 tonnes**
* Average profit: **₹817,187.99**

Chilli has an average profit of approximately **₹750,878.34**.

### State Performance

Punjab has the highest average profit among the states analyzed, at approximately **₹136,025.64**, followed closely by Maharashtra and Karnataka.

### Water Efficiency

Sugarcane has the highest average water-efficiency value in the dataset:

**30.48 tonnes per 1,000 m³**.

### Irrigation

The average yields by irrigation method are:

| Irrigation Method | Average Yield (Tonnes/Ha) |
| ----------------- | ------------------------: |
| Drip              |                      6.58 |
| Sprinkler         |                      5.16 |
| Flood             |                      4.86 |
| Rainfed           |                      4.60 |

These are descriptive results from the dataset and do not by themselves establish that irrigation method causes the observed yield differences.

---

## 📁 Output Files

The analysis generates three summary CSV files:

```text
seasonal_summary.csv
crop_analysis.csv
state_analysis.csv
```

These files contain summarized seasonal, crop-wise, and state-wise performance results.

---

## ▶️ How to Run the Project

### 1. Install Python

Install Python 3.x on your system.

### 2. Install Required Libraries

```bash
pip install pandas numpy matplotlib seaborn
```

### 3. Place the Dataset

Keep the dataset in the project directory:

```text
seasonal_agriculture_performance_dataset.csv
```

### 4. Update the File Path

If running locally, change the dataset path in the Python program:

```python
file_path = "seasonal_agriculture_performance_dataset.csv"
```

The original analysis loads the dataset from Google Drive/Colab.

### 5. Run the Python File / Notebook

Execute the Python code to perform:

```text
Data Loading
     ↓
Data Cleaning
     ↓
EDA
     ↓
Visualization
     ↓
Correlation Analysis
     ↓
Performance Analysis
     ↓
CSV Report Generation
```

---

## 👥 End Users

This project can be useful for:

* Farmers
* Agricultural analysts
* Agribusiness teams
* Agricultural researchers
* Data analysts
* Agricultural planners
* Resource-management teams
* Students and academic researchers

---

## 🚀 Future Scope

The project can be extended by adding:

* Machine learning models for yield prediction
* Crop recommendation systems
* Weather-based crop forecasting
* Disease and pest prediction
* Automated irrigation recommendations
* Interactive Power BI/Tableau dashboards
* Real-time agricultural data
* Satellite and remote-sensing data
* Soil-quality prediction
* Profit prediction models
* Time-series analysis
* IoT-based farm monitoring

---

## ⚠️ Limitations

* The analysis is based on the provided dataset.
* The project mainly performs descriptive and exploratory analysis.
* Correlation does not establish causation.
* The dataset may not represent every agricultural region or farming condition.
* Predictions would require additional modeling and validation.

---

## 📌 Conclusion

The **Seasonal Agriculture Performance Analysis** project demonstrates how Python can be used to analyze agricultural data and identify patterns related to **seasonal performance, crop yield, production, profitability, irrigation, environmental conditions, water efficiency, and disease/pest risk**.

The project combines **Pandas and NumPy for data processing** with **Matplotlib and Seaborn for visualization**, producing analytical summaries and CSV outputs that can be used for further agricultural analysis.

---

## 👨‍💻 Project Type

**Data Analytics / Exploratory Data Analysis / Agricultural Data Analysis**

### Technologies

```text
Python
Pandas
NumPy
Matplotlib
Seaborn
Google Colab / Jupyter Notebook
CSV
```
