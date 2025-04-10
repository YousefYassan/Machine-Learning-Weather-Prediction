# Machine-Learning-Weather-Prediction
![rain (1)](https://github.com/user-attachments/assets/f67e7e08-67a5-4793-8c6a-d80fb9f9f89a)

##Weather Prediction Project
Overview
This machine learning project predicts whether it will rain tomorrow based on today's weather parameters. The system uses a Random Forest classifier model that has been trained on historical weather data, delivering 88% accuracy in rainfall prediction.
Features

#Dual User Interfaces:

Tkinter GUI: Desktop application for local use
Streamlit Web App: Browser-based interface for easy access


Machine Learning Model: Random Forest classifier with superior performance metrics
Data Processing: Sophisticated encoding for categorical features including wind direction and rain status
Temporal Feature Engineering: Utilizes date-based features for improved prediction accuracy


The project includes comprehensive data visualization and analysis:

Correlation matrices showing relationships between weather parameters
Temperature distribution histograms
Feature importance visualization
Model performance comparisons

#Installation
Prerequisites

Python 3.10 or higher
Required dependencies

Setup

Clone the repository
Install dependencies:

pip install -r requirements.txt
Dependencies

tkinter
streamlit
numpy
pillow
joblib
scikit-learn
matplotlib
pandas

Usage
Running the Tkinter GUI
python weather\ gui.py
Running the Streamlit Web App
streamlit run WeatherGuiStreamlit.py
How It Works

Data Input: User provides current weather parameters through either interface
Data Processing:

Categorical encoding (wind direction, rain status)
Temporal feature extraction (year, month, day, weekday)
Feature normalization


Prediction: The trained Random Forest model predicts rainfall likelihood
Output: Results are displayed to the user with a clear Yes/No answer

Technical Details
Model Architecture
The project uses a Random Forest Classifier that:

Handles non-linear relationships in weather data
Prevents overfitting through ensemble learning
Captures complex interactions between weather parameters

Feature Engineering

Wind direction encoding using trigonometric functions (sin/cos)
Binary encoding for rain status
Date-based feature extraction

Model Performance
ModelAccuracyPrecisionRecallF1-ScoreRandom Forest88%86%85%85.5%XGBoost87%85%84%84.2%SVM82%80%78%78.5%Logistic Regression79%77%75%75.8%
Key Features by Importance

Humidity (3pm)
Pressure (3pm)
Rainfall
Temperature (3pm)
Wind speed/direction

Project Structure
├── weather gui.py            # Tkinter-based GUI
├── WeatherGuiStreamlit.py    # Streamlit web app
├── weather predection.ipynb  # Jupyter Notebook (Data Exploration & Model Training)
├── random_forest_model.pkl   # Trained machine learning model
├── rain.jpg                  # UI background image
└── requirements.txt          # Dependencies
Future Improvements
![Screenshot 2025-02-18 092159](https://github.com/user-attachments/assets/4607cd74-e0cd-42ea-ac14-ab9e08623eae)
![Screenshot 2025-02-18 092208](https://github.com/user-attachments/assets/eaa3da40-767f-4052-b95e-c5011f146bcb)
![Screenshot 2025-02-18 092213](https://github.com/user-attachments/assets/173326ae-98b2-466b-a29e-0ce0095c5371)

Enhanced model accuracy with additional weather parameters
Cloud deployment of the Streamlit application
Interactive data visualizations and predictive analytics
Integration with real-time weather API data
Mobile application development
