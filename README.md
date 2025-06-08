# ☀️ Solar Storm Impact: Power Grid Disruption Prediction

This project focuses on predicting the severity of power grid disruptions caused by solar storms using historical and simulated space weather data. It combines classification models like Random Forest, XGBoost, and SVM within a full machine learning pipeline — from preprocessing to model evaluation and leaderboard comparison.

---

## 📌 Project Overview

Solar storms can seriously affect power grids, satellite communication, and GPS systems. This project aims to support early warning systems by:

* Predicting the severity of power grid disruption (None, Minor, Moderate, Severe)
* Identifying key solar storm features impacting the grid
* Building a robust ML pipeline for disaster prediction

---

## 🧠 Features & Techniques

* ✅ Data Simulation & Loading (realistic solar weather patterns)
* ✅ Data Cleaning and Preprocessing (type casting, scaling, encoding)
* ✅ Feature Engineering (flare metrics, wind properties)
* ✅ Exploratory Data Analysis (correlation matrix, feature distribution)
* ✅ Classification Models (Random Forest, XGBoost, SVM)
* ✅ Model Comparison Leaderboard (accuracy, precision, recall, F1)
* ✅ Confusion Matrix Visualization

---

## 📂 Dataset

The **Solar Storm Power Grid Impact Dataset** includes 1,000 rows × 9 columns:

| Feature                  | Description                                                      |
| ------------------------ | ---------------------------------------------------------------- |
| `event_id`               | Unique identifier for the solar storm                            |
| `event_date`             | Date of occurrence                                               |
| `solar_flare_class`      | Solar flare class (C, M, X)                                      |
| `flare_intensity`        | Intensity score on a 1–100 scale                                 |
| `geomagnetic_index_Kp`   | Geomagnetic storm index (0–9)                                    |
| `solar_wind_speed`       | Solar wind speed (km/s)                                          |
| `solar_wind_density`     | Solar wind density (particles/cm³)                               |
| `flare_duration_minutes` | Duration of flare                                                |
| `power_grid_disruption`  | Disruption level (Target: 0=None, 1=Minor, 2=Moderate, 3=Severe) |

---

## 🛠️ Tech Stack

* **Language**: Python
* **Libraries**:

  * `pandas`, `numpy`
  * `matplotlib`, `seaborn`
  * `scikit-learn`, `xgboost`
  * `datetime`, `plotly`

---

## 📊 Exploratory Data Analysis

* Histograms for flare intensity, wind speed, and Kp index
* Class balance for disruption levels
* Heatmap showing feature correlation
* Box plots showing feature behavior across disruption levels

---

## 📈 Models Implemented

| Model         | Description                     | F1-Score (Macro) |
| ------------- | ------------------------------- | ---------------- |
| Random Forest | Baseline classifier             | \~0.92           |
| XGBoost       | Gradient-boosted decision trees | \~0.93 ✅         |
| SVM           | Support Vector Machine (RBF)    | \~0.87           |

---

## 🧪 Evaluation Metrics

* ✔️ Accuracy
* 📉 Confusion Matrix
* 📊 Precision, Recall, F1 (Macro Averaged)
* 🏆 Visual Leaderboard using `seaborn`

---

## ✅ Key Findings

* **XGBoost** performed the best, making it ideal for high-impact solar storm prediction.
* `geomagnetic_index_Kp`, `solar_wind_speed`, and `flare_intensity` were most influential.
* Severe disruptions are rarer, making macro metrics crucial.

---

## 🚀 Getting Started

1. **Clone the repository**

   ```bash
   git clone https://github.com/Souvik-Rana/Solar-Storm-PowerGrid-Prediction.git
   cd Solar-Storm-PowerGrid-Prediction
   ```

2. **Install dependencies**

   ```bash
   pip install -r requirements.txt
   ```

3. **Run the Jupyter Notebook**
   Open `solar_storm_prediction.ipynb` and execute the cells.

---

## ✅ Future Enhancements

* Add time-series forecasting using solar activity data
* Integrate satellite telemetry (e.g., NOAA, NASA) for real-world prediction
* Build a real-time alert dashboard using `Streamlit`

---

## 🔗 Dataset Provenance

*This dataset was simulated using scientific references and NOAA/NASA-style solar weather patterns. While not real satellite data, it mimics plausible values of historical solar storm events for educational and ML benchmarking purposes.*

---

## 👤 Author

<p align="center">
  <b> SOUVIK RANA </b><br>
  <br><a href="https://github.com/Souvik-Rana">
    <img src="https://img.shields.io/badge/GitHub-000?style=for-the-badge&logo=github&logoColor=white" />
  </a>
  <a href="https://www.linkedin.com/in/souvik-rana-19a797221/">
    <img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" />
  </a>
  <a href="https://www.kaggle.com/souvikrana">
    <img src="https://img.shields.io/badge/Kaggle-20BEFF?style=for-the-badge&logo=kaggle&logoColor=white" />
  </a>
  <a href="https://souvik-rana.vercel.app">
    <img src="https://img.shields.io/badge/Portfolio-FF5722?style=for-the-badge&logo=Firefox&logoColor=white" />
  </a>
</p>

<p align="center">
  <img src="https://github.com/Souvik-Rana/Souvik-Rana/blob/e7e77b01346caa8d86d548a54ffeb41716a210b6/SOUVIK%20RANA%20BANNER.png" alt="Project Banner" width="100%">
</p>

---

## 🤝 Contributions

Contributions, ideas, and feedback are welcome. Fork this repo, open issues, or submit pull requests to collaborate!
