                                                                              Project Workflow
1. ### Data Loading
Imported the dataset (Iris.csv) and reviewed its structure.
Removed the ID column, as it doesn't contribute to the classification task.
Encoded species labels into numerical values for model training.
2. ### Exploratory Data Analysis (EDA)
Visualized feature relationships using a pair plot.
Observed clear separability of the Setosa species and some overlap between Versicolor and Virginica.
3. ### Data Preprocessing
Split the dataset into:
Features (X): Sepal and petal dimensions.
Target (y): Species labels.
Divided data into training (80%) and testing (20%) sets.
4. ### Model Training
Trained a Random Forest Classifier due to its robustness and ability to handle overlapping classes.
Tuned hyperparameters for optimal accuracy.
5. ### Model Evaluation
Achieved high accuracy on the test set.
Evaluated performance using:
Confusion Matrix: To visualize true vs. predicted classes.
Classification Report: For precision, recall, and F1-score.
6.### Feature Importance Analysis
Analyzed the contribution of each feature (sepal/petal dimensions) to the model's decision-making process.
Observed that petal length and petal width are the most significant features.
7.### Predictions on New Data
Used the trained model to predict species for new flower measurements:
Example Input: [5.1, 3.5, 1.4, 0.2]
Predicted Output: Setosa
8. ### Model Saving
Saved the trained model as iris_model.pkl for future use or deployment.
