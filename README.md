## Predicting Ship Energy Consumption Using Machine Learning 🚢⚡
# Overview
This project explores machine learning techniques to predict the energy consumption of a Danish ro-ro passenger ship based on real-world sensor data. By analyzing key parameters such as ship speed, rudder angles, and pitch values, the model helps optimize fuel efficiency, reduce costs, and minimize environmental impact.

# Dataset
The dataset consists of time-series records from various sensors, including:

Fuel properties (density, volume flow rate, temperature)
Ship navigation (speed, rudder angles, track degree, heading)
Environmental factors (wind speed, wind angle)
The energy consumption is calculated using:

𝐸𝐶 = fuelDensity × (fuelVolumeFlowRate × 3600 × 24) / 1000 (tons/day)

For this project, consumption is calculated at 5-minute intervals.

# Preprocessing Steps
✔ Merged multiple CSV files into a single dataset \n
✔ Converted timestamps from .NET ticks to datetime \n
✔ Resampled data at 5-minute intervals \n
✔ Handled missing values and selected relevant features \n
✔ Scaled numerical features using StandardScaler \n

# Models Used
The following regression models were trained and compared:

Decision Tree 🌳 (baseline)
Random Forest 🌲🌲 (improved generalization)
Gradient Boosting 🚀 (best performance)
Results & Insights
📊 Gradient Boosting outperformed other models, achieving higher accuracy and lower RMSE.
📉 Scatterplots of actual vs predicted energy consumption showed better alignment for Gradient Boosting.
💡 Feature importance analysis revealed that speed, rudder angles, and propeller pitch were key drivers of fuel consumption.

# Visualization
Here’s an example scatterplot comparing actual vs predicted values:
(Add an image link here if you have one)

# Future Improvements
🔹 Experiment with deep learning models (e.g., LSTMs for time-series)
🔹 Optimize feature selection & hyperparameters further
🔹 Extend dataset with real-time ship monitoring data

# Contributing
Feel free to fork this repo, open issues, or submit pull requests if you have improvements! 🚢💡

# Contact
🔗 Connect with me on LinkedIn - https://www.linkedin.com/in/ifeanyi-agu-099b5a197/
📧 Email: aaifeanyi20@outlook.com
