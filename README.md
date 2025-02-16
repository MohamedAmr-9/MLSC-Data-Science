**Predictions herein deal with Hazardous NEOs (Nearest Earth Objects).**

📌 Project Description

Objectives of the Project: To predict whether a Near-Earth Object (NEO) is hazardous based on historical NEO data from NASA from 1910 to 2024. It comprises different attributes like magnitude, diameter, velocity, and distance from the Earth; the dataset consists of over 338,000 records.

📂 Dataset

Source: NASA NEO Dataset (1910-2024)
Number of Records: 338,199
Target Variable: is_hazardous (0 = Not Hazardous, 1 = Hazardous)

🛠 Project Workflow

Pre-Processing and Cleaning of Data
Remove missing values.
Selection of features.
Encoding of categorical variables.
Scaling numerical features.
Make classes move toward balance by handling imbalance using SMOTE.
Exploratory Data Analysis (EDA)
Visual Distribution of Hazardous vs. Non-Hazardous Objects
Understanding key features using correlation and plots
Model Training and Evaluation
Model built on training RandomForestClassifier.
Evaluated model based on: 
- Precision 
- Recall 
- F1-Score
Area Under the Curve (AUC-ROC) score.
Confusion Matrix.
Model Deployment
The model was saved as a trained model (neo_hazard_predictor.pkl).
Scaler was saved for future data normalization (scaler.pkl)
Function to make predictions on new data

📊 Results

The model was able to effectively predict hazardous NEOs.
Model balanced classes by SMOTE and scaling.
Visualized key features affecting predictions with a feature importance plot.

🚀 How to Use

Get a clone of this repository
cd neo-hazard-prediction
Install the dependencies
pip install -r requirements.txt
Now run the Jupyter Notebook for exploratory look through the project
While using the model, saved it for future

📌 Future Improvements

Test with more models, e.g., XGBoost, SVM
Deep learning models should be considered to further improve accuracy
Live predictions through incorporation of real-time data from NASA.

📝 Author
Developed By Mohamded Amr Mohamed Tolba part of the MLSC Data Science Graduation Project.

🚀 Happy Coding! 
