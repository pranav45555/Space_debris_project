# 🛰 CosmicGuard: Space Debris Collision Prediction System

CosmicGuard is an AI-powered Space Situational Awareness (SSA) system
designed to predict potential collisions between operational satellites
and orbital debris. It combines orbital mechanics (SGP4 propagation)
with machine learning models to estimate collision probability, classify
risk levels, and forecast future object positions.

------------------------------------------------------------------------

## 🚀 Key Features

-   Predicts collision probability between satellites and debris
-   Classifies risk levels: Low / Medium / High
-   Forecasts future orbital coordinates using SGP4
-   Supports ML models: Logistic Regression, SVM, Random Forest
-   Hybrid prediction architecture: SGP4 + Random Forest + LSTM
-   Generates analytical visualizations and insights
-   Provides decision-support reporting for mission planning

------------------------------------------------------------------------

## 🎯 Project Objectives

The system aims to:

-   Predict satellite--debris collision probability
-   Estimate minimum separation distance
-   Forecast future orbital trajectories
-   Classify collision threat levels
-   Improve space situational awareness using AI techniques

------------------------------------------------------------------------

## 🧠 Model Architecture

Pipeline:

TLE Dataset → SGP4 Propagation → Feature Engineering → ML Models →
Collision Probability → Risk Classification → Future Position Prediction

------------------------------------------------------------------------

## 📊 Model Outputs

Outputs include:

-   Collision Probability Score
-   Risk Classification (Low / Medium / High)
-   Future Position Coordinates (x, y, z)

Example:

Collision Probability: 0.82\
Risk Level: HIGH\
Future Coordinates: (4213, −1287, 5320)

------------------------------------------------------------------------

## 📂 Project Structure

cosmicguard/ │ ├── data/ ├── notebooks/ ├── models/ ├── utils/ ├──
train_model.py ├── predict.py ├── main.py └── README.md

------------------------------------------------------------------------

## 📥 Datasets Used

Supported datasets:

-   CelesTrak TLE Dataset
-   Conjunction Data Messages (CDM)
-   ESA DISCOS Database (optional)

These datasets provide orbital parameters, relative velocity, miss
distance, time-to-closest approach, and object size.

------------------------------------------------------------------------

## ⚙️ Installation

Clone repository:

git clone https://github.com/yourusername/cosmicguard.git cd cosmicguard

Install dependencies:

pip install pandas numpy scikit-learn matplotlib seaborn sgp4 joblib
tensorflow

------------------------------------------------------------------------

## ▶️ Usage

Train model:

python train_model.py

Run prediction:

python predict.py

------------------------------------------------------------------------

## 📈 Evaluation Metrics

Models are evaluated using:

-   Accuracy
-   Precision
-   Recall
-   F1-score
-   ROC-AUC
-   RMSE (trajectory prediction)
-   Miss-distance estimation error

------------------------------------------------------------------------

## 🧪 Algorithms Used

Baseline Models:

-   Logistic Regression
-   Support Vector Machine (SVM)
-   Random Forest

Trajectory Prediction:

-   SGP4 Orbit Propagation

Advanced Hybrid Model:

SGP4 + Random Forest + LSTM

------------------------------------------------------------------------

## 🌍 Applications

-   Satellite mission planning
-   Collision avoidance strategy support
-   Space situational awareness systems
-   Orbital risk monitoring platforms
-   Aerospace analytics research

------------------------------------------------------------------------

## 🔮 Future Enhancements

-   Real-time debris tracking integration
-   Transformer-based trajectory prediction
-   3D orbit visualization using CesiumJS
-   Automated model retraining pipeline
-   Collision avoidance maneuver simulation
-   Web dashboard deployment

------------------------------------------------------------------------

## 👨‍💻 Contributors

Developed as part of an academic capstone project applying Artificial
Intelligence and orbital analytics to improve satellite safety and
mitigate risks caused by space debris in Earth orbit.
