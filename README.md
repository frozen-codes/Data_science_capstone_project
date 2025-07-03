🚀 SpaceX Launch Site Analysis & First Stage Landing Prediction
This project is part of the IBM Data Science Capstone and explores the SpaceX Falcon 9 first stage landing success prediction using various machine learning models and visualizes launch site insights using Folium interactive maps.

📌 Table of Contents
📖 Project Description

📂 Project Structure

🔍 Tasks Overview

📊 Visualizations with Folium

🧠 Machine Learning Models

📈 Results & Evaluation

🛠 Technologies Used

📁 Dataset

📌 How to Run

📜 License

📖 Project Description
SpaceX has developed reusable rockets that can land back safely after delivering payloads to space. This project aims to:

Understand geospatial factors affecting launch site locations.

Visualize launch outcomes and their locations interactively.

Predict whether the first stage of the rocket lands successfully using historical data and supervised machine learning techniques.

📂 Project Structure
bash
Copy
Edit
SpaceX-Landing-Prediction/
├── spacex_launch_geo.csv
├── SpaceX_Landing_Analysis.ipynb   # Interactive map visualizations
├── Model_Training_Prediction.ipynb # ML training and evaluation
├── presentation.pdf                # Final summary presentation (optional)
├── README.md                       # This file
└── requirements.txt                # Python dependencies
🔍 Tasks Overview
Task 1: Mark All Launch Sites
Plotted NASA JSC and all SpaceX launch sites using Folium Map, folium.Circle, and folium.Marker.

Task 2: Mark Launch Success & Failures
Colored markers for each launch:
🟢 Green = Success
🔴 Red = Failure

Task 3: Proximity Distance Analysis
Measured distances from launch sites to:

Coastlines

Railways

Cities

Highways

Used haversine formula and displayed with folium.PolyLine.

📊 Visualizations with Folium
Interactive map visualizations help to:

Understand the proximity of launch sites to key infrastructure.

Analyze patterns of launch outcomes geographically.

Identify optimal launch site conditions visually.

🧠 Machine Learning Models
The following models were trained and evaluated:

Logistic Regression

Support Vector Machines (SVM)

Decision Tree Classifier

K-Nearest Neighbors (KNN)

Techniques Applied:
Feature standardization

Train/Test split

GridSearchCV for hyperparameter tuning (with cv=10)

📈 Results & Evaluation
Model	Accuracy Score
Logistic Regression	83.33%
SVM	84.72%
Decision Tree	81.94%
KNN	75.00%

✅ SVM performed best based on test set accuracy.

🛠 Technologies Used
Python 3.10+

Pandas, NumPy

Folium, Matplotlib, Seaborn

scikit-learn

Jupyter Notebook

📁 Dataset
📄 spacex_launch_geo.csv: Provided by IBM via IBM Skills Network

Includes columns such as:

Launch Site, Lat, Long, class, Orbit, Payload Mass (kg), etc.

📌 How to Run
Clone the repository:

bash
Copy
Edit
git clone https://github.com/your-username/spacex-landing-prediction.git
cd spacex-landing-prediction
Install dependencies:

bash
Copy
Edit
pip install -r requirements.txt
Open Jupyter Notebook and run:

SpaceX_Landing_Analysis.ipynb

Model_Training_Prediction.ipynb

📜 License
This project is licensed under the MIT License.
Feel free to use and adapt for learning and research purposes.

🚀 Contributed by: [Your Name]
