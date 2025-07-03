# 🚀 SpaceX Falcon 9 First Stage Landing Prediction & Interactive Visual Analytics

This project is a comprehensive data science and interactive geospatial analytics solution built using **Machine Learning**, **Folium**, and **Plotly Dash**. It aims to:
- Predict the **landing success** of Falcon 9 first stages
- Visualize and analyze the **geographical impact** of launch site locations on mission outcomes

---

## 📌 Project Objectives

### Part 1: Landing Prediction (ML)
- Perform Exploratory Data Analysis (EDA)
- Preprocess and standardize the dataset
- Train & evaluate multiple classification models:
  - Logistic Regression
  - Support Vector Machine (SVM)
  - Decision Tree
  - K-Nearest Neighbors (KNN)
- Optimize using GridSearchCV
- Select the best-performing model based on test accuracy

### Part 2: Visual Analytics (Folium)
- Mark all launch sites on an interactive map
- Display success and failure of each launch
- Calculate and annotate distances from launch sites to:
  - Coastlines
  - Railways
  - Highways
  - Cities

---

## 🗃️ Project Structure

```bash
SpaceX-Launch-Prediction/
├── data/
│   └── spacex_launch_geo.csv
│   └── spacex_df.csv
├── notebooks/
│   └── SpaceX_Landing_Prediction.ipynb
│   └── Interactive_Map_Visualization.ipynb
├── images/
│   └── map_markers.png
│   └── distance_lines.png
├── README.md
└── requirements.txt


## 📊 Model Performance Summary

| Model                 | Test Accuracy |
|----------------------|---------------|
| Logistic Regression  | 87%           |
| SVM (RBF Kernel)     | 92% ✅        |
| Decision Tree        | 89%           |
| K-Nearest Neighbors  | 90%           |

> ✅ **Support Vector Machine (SVM) with RBF Kernel** achieved the highest accuracy.

---

## 🌍 Interactive Map Highlights

- Launch site markers placed using `folium.Circle` and `folium.Marker`
- Success (🟢 green) and failure (🔴 red) launches differentiated by color
- Distance to closest:
  - Coastlines
  - Railways
  - Highways
  - Cities
- Added:
  - Popup labels
  - Mouse position coordinate tracking
  - PolyLines showing distances

---

## 📸 Screenshots

### 🔹 Launch Site Markers
![Launch Sites](images/map_markers.png)

### 🔹 Distance to Coastline
![Distance Line](images/distance_lines.png)

---

## 🔍 Key Insights

- Most launch sites are located:
  - **Close to the Equator** for better orbital velocity
  - **Near the coast** for safe landings over oceans
  - **Close to infrastructure** like roads and railways
- Launch site geography impacts success probability
- SVM outperforms other models for this dataset

---

## ▶️ Getting Started

### 1. Clone the repository
```bash
git clone https://github.com/yourusername/SpaceX-Launch-Analysis.git
cd SpaceX-Launch-Analysis
SpaceX_Landing_Analysis.ipynb

Model_Training_Prediction.ipynb

📜 License
This project is licensed under the MIT License.
Feel free to use and adapt for learning and research purposes.

🚀 Contributed by: Suraj 
