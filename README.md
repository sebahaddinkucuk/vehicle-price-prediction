# Vehicle Price Prediction

A machine learning project for vehicle listing data collection, data preprocessing, exploratory data analysis, and vehicle price prediction using an artificial neural network.

## Project Overview

This project explores vehicle listing data to identify pricing patterns and estimate vehicle prices based on vehicle characteristics and condition.

It includes data collection, data analysis, feature engineering, model training, model evaluation, and a simulation for analyzing how changes in vehicle body-part condition may affect predicted prices.

## Project Files

### `tflite.ipynb`
The main notebook containing the core project workflow, including data preprocessing, feature engineering, artificial neural network training, model evaluation, TensorFlow Lite export, and vehicle price prediction and damage simulation.

### `Veri(1).ipynb`
A notebook used to collect vehicle listing data for further analysis and model development.

### `7.dacia(1).xls`
An example vehicle dataset containing listing information used for data exploration and experimentation.

## Key Features

- Vehicle listing data collection
- Data cleaning and preprocessing
- Exploratory data analysis and statistical visualizations
- Vehicle age and reference price calculation
- Weighted vehicle damage scoring
- Artificial neural network training with TensorFlow/Keras
- Model evaluation using R² score and Mean Absolute Error (MAE)
- TensorFlow Lite model export
- Vehicle price prediction and damage-condition simulation

## Technologies Used

- Python
- Jupyter Notebook
- Pandas
- NumPy
- Scikit-learn
- TensorFlow / Keras
- TensorFlow Lite
- Matplotlib
- Seaborn

## Model Workflow

1. Collect and load vehicle listing data.
2. Clean numerical values and handle missing or invalid records.
3. Calculate vehicle age and group-based reference prices.
4. Encode categorical features and calculate weighted damage scores.
5. Scale model inputs and apply logarithmic price transformation.
6. Train an artificial neural network.
7. Evaluate model performance using R² score and MAE.
8. Export the trained model to TensorFlow Lite.
9. Simulate vehicle condition changes and compare price predictions.

## Model Input Features

The model uses the following features:

- **Mileage:** Total distance traveled by the vehicle.
- **Vehicle Age:** Age calculated from the model year.
- **Reference Price:** Median price for a vehicle group.
- **Encoded Color:** Numerical representation of vehicle color.
- **Damage Score:** Weighted score based on vehicle body-part condition.

## Evaluation Metrics

- **R² Score:** Measures how well the model explains variation in vehicle prices.
- **Mean Absolute Error (MAE):** Measures the average absolute difference between predicted and actual prices.

Model performance depends on the dataset, data quality, and training configuration.

## Getting Started

### Requirements

Install the required Python libraries:

```bash
pip install pandas numpy scikit-learn tensorflow matplotlib seaborn
```

### Running the Project

1. Open `Veri(1).ipynb` to review the data collection workflow.
2. Open `tflite.ipynb` to explore the preprocessing, analysis, model training, and prediction workflow.
3. Ensure the dataset filename and file paths in the notebook match the files available in your environment.
4. Run the notebook cells in order.

## Dataset

The project uses vehicle listing information, including prices, mileage, model years, brands, models, colors, and vehicle condition.

The example dataset is provided for experimentation. Please ensure that redistribution of collected listing data is permitted by the original website's terms and applicable rules.

## Future Improvements

- Improve model validation and prevent data leakage.
- Compare different machine learning algorithms.
- Improve handling of unseen vehicle categories.
- Develop an interactive interface for price prediction.

## Disclaimer

This project is intended for educational and experimental purposes. Predicted prices are estimates and are not guaranteed market values.

## Author

Computer Engineering Student | Machine Learning & Artificial Intelligence
