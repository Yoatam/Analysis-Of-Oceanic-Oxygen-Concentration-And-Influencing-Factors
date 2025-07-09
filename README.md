# Oceanic Oxygen Concentration Analysis
# 🌊 Ocean Oxygen Analysis

This project examines how **temperature**, **salinity**, and **depth** influence **oxygen levels in the ocean** — a crucial question for understanding marine ecosystems, climate change, and environmental sustainability.

Our team worked with real-world oceanographic data to **clean**, **visualize**, and **model** the key environmental factors influencing oxygen concentration in seawater. We applied both **statistical** and **machine learning techniques** to find patterns and make accurate predictions.

---

## 📌 Project Overview

Oxygen levels in seawater are crucial for the survival of marine life, the health of the ocean, and the global climate. This analysis investigates how physical ocean properties — particularly **depth**, **temperature**, and **salinity** — influence oxygen concentration in the ocean.

We built predictive models and performed exploratory analysis to understand these relationships and their implications.

---

## ❓ Key Questions

- What are the most influential factors affecting oxygen levels in the ocean?
- How are oxygen levels distributed across different depths and time periods?
- Can we build reliable models to predict oxygen concentration using environmental data?

---

## 📂 Dataset

- **504 observations** from ocean sensors and sample bottles.

### Key Variables

- `CTDTEMP`: Temperature of seawater  
- `CTDSAL`: Salinity of seawater  
- `depth`: Depth in meters  
- `micromoles_of_oxygen_per_unit_mass_in_sea_water`: Oxygen concentration  
- `Latitude`, `Longitude`: (not fully analyzed due to merging complexity)

---

## ⚙️ Methods

### 🔧 Data Cleaning

- Filled missing values with column means  
- Removed outliers using Z-score filtering

### 📊 Exploratory Data Analysis (EDA)

- Correlation analysis and hypothesis testing  
- Pairplots, scatter plots, time series visualization

### 🤖 Modeling

- **Random Forest Regression** (best performer)  
- **Linear Regression** (baseline comparison)  
- Cross-validation for performance stability

---

## 🔍 Key Findings

- **Depth** was the most important factor — deeper waters had significantly lower oxygen levels.
- **Temperature** and **salinity** also impacted oxygen concentration, though less strongly than depth.
- **Random Forest models** outperformed others due to their ability to capture non-linear patterns.
- **Cross-validation** confirmed model stability, with a mean R² of approximately **0.85**.

---

## ⚠️ Limitations

- Geographic factors (latitude, longitude) were not fully explored due to data merging issues.
- The dataset lacked variables such as **ocean currents** and **biological activity**, which could improve future models.
- Time series analysis was limited; future work could explore **seasonal** and **long-term trends**.

---

## ▶️ How to Run

1. **Clone this repository**:
   ```bash
   git clone https://github.com/your-username/your-repo-name.git
   cd your-repo-name

### 🙌 Acknowledgments
Thanks to oceanographic institutions and open-data initiatives for providing the dataset that made this analysis possible.
