# Iris-Flower-Classification


## Project Overview
The Iris Flower Classification project aims to classify iris flowers into three species: Setosa, Versicolor, and Virginica, using their sepal and petal dimensions. This project utilizes the Random Forest Classifier for classification and explores key steps in data preprocessing, visualization, and machine learning.

## Dataset Information
Source: Provided as Iris.csv.

Columns:

ID: Unique identifier (dropped during preprocessing).

SepalLengthCm: Length of the sepal in cm.

SepalWidthCm: Width of the sepal in cm.

PetalLengthCm: Length of the petal in cm.

PetalWidthCm: Width of the petal in cm.

Species: Target class (Setosa, Versicolor, Virginica).

## Project Workflow

Step 1: Data Loading and Preprocessing

Loaded the dataset using pandas and displayed basic information.

Dropped the ID column as it was irrelevant for classification.

Checked for missing values (none found).

Encoded the Species column using LabelEncoder:

Setosa → 0

Versicolor → 1

Virginica → 2

Step 2: Exploratory Data Analysis (EDA)

Used seaborn pair plot to visualize feature relationships.

Highlighted distinctions between species based on sepal and petal measurements.

Step 3: Data Splitting

Split the dataset into features (X) and target (y).

Divided the data into training (80%) and testing (20%) sets using train_test_split.

Step 4: Model Training

Used a Random Forest Classifier:

Randomized tree-based ensemble method for robust classification.

Trained the model on the training dataset.

Step 5: Model Evaluation

Predicted the test set outcomes.

Evaluated the model:

Accuracy: High accuracy on the test data.

Classification Report: Displayed precision, recall, and F1 scores for each class.

Confusion Matrix: Highlighted classification errors using a heatmap.

Step 6: Feature Importance Analysis

Analyzed feature importance:
Visualized contributions of sepal and petal dimensions to the model's decision-making process.

Step 7: Prediction on New Data

Tested the model with new flower measurements:

Example inputs:

[5.1, 3.5, 1.4, 0.2] → Predicted Setosa.

[6.7, 3.0, 5.2, 2.3] → Predicted Virginica.

Converted numeric predictions back to species names using the encoder.

Step 8: Model Saving

Saved the trained model as iris_model.pkl using joblib.

Ensured the model can be loaded for future predictions.

## Key Libraries Used

pandas: For data loading and manipulation.

seaborn & matplotlib: For data visualization.

scikit-learn: For data preprocessing, model training, evaluation, and splitting.

joblib: For model serialization.

