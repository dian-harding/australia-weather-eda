# Exploratory Data Analysis: Australian Rainfall & Weather Patterns (2016)

## 📌 Project Overview
An exploratory data analysis (EDA) examining daily weather observations across Australia during 2016. The project focuses on the relationship between atmospheric variables (temperature, humidity) and precipitation, regional rainfall distribution, and variance across major metropolitan regions.

---

## 📊 Dataset & Lineage
* **Dataset Name:** Rain in Australia (`weatherAUS.csv`)
* **Curator / Uploader:** Joe Young via [Kaggle](https://www.kaggle.com/datasets/jsphyg/weather-dataset-rattle-package)
* **Primary Source:** Australian Commonwealth Bureau of Meteorology (BOM), processed via Graham Williams' Rattle toolkit
* **Scope:** Daily meteorological observations across Australia for the calendar year 2016

---

## 🔍 Key Findings & Insights

1. **Humidity & Temperature Dynamics:**
   * Precipitation events heavily cluster in environments with 3 PM relative humidity exceeding **60%**.
   * Dry conditions dominate higher temperature ranges with low afternoon humidity.

2. **Distribution Skewness:**
   * Daily rainfall is heavily right-skewed. The median precipitation on rainy days is **4.8 mm**, whereas the mean is pulled to **8.78 mm** due to extreme rainfall events exceeding 80–100 mm.

3. **Geographical & Volume Discrepancies:**
   * **Highest Volume:** Darwin (1,064.4 mm) and Sydney (1,068.0 mm) recorded the highest total accumulation.
   * **Frequency vs. Volume:** Hobart recorded the highest count of rainy days (159 days), followed by Melbourne Airport (154 days), indicating a regime characterized by frequent light drizzle rather than high-volume downpours.
   * **Arid Regions:** Alice Springs and Woomera consistently exhibited the lowest rainfall frequencies (8–10 days) and totals (<60 mm).

4. **Metropolitan Variance:**
   * **Sydney** shows the widest interquartile range (IQR) and several high outliers (>80 mm).
   * **Melbourne** demonstrates minimal spread and low outlier ceilings (<25 mm), reflecting consistent low-intensity precipitation.

---

## 🛠️ Tech Stack & Methods
* **Language:** R (v4.x)
* **Libraries:** `dplyr`, `base graphics`
* **Techniques:** Data filtering, metric aggregation, random sampling, distribution profiling (density histograms, boxplots).

---

## 📂 Repository Structure

```text
├── README.md                           # Project summary and key insights
├── weather_australia_analysis.Rmd      # Source R Markdown analysis
├── weatherAUS.csv                      # Dataset (Kaggle: Rain in Australia)
```

---

## 🚀 How to Run the Analysis

1. Clone this repository:
   ```bash
   git clone https://github.com/<your-username>/australia-weather-eda.git
   ```
2. Place `weatherAUS.csv` in the root folder.
3. Open `weather_australia_analysis.Rmd` in RStudio.
4. Click **Knit** to compile to HTML or PDF.