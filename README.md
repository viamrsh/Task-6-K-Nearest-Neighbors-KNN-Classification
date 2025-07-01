# Task-6-K-Nearest-Neighbors-KNN-Classification
1.Choose a classification dataset and normalize features.

2.Use KNeighborsClassifier from sklearn.

3.Experiment with different values of K.

4.Evaluate model using accuracy, confusion matrix.

5.Visualize decision boundaries.

---

# Objective:
Understand and implement KNN for classification problems.

---
# Tools:
Scikit-learn, Pandas, Matplotlib

---
# code explanation 


---

Step 1: Import Libraries

You import essential libraries for:

Data handling (pandas, numpy)

Plotting (matplotlib)

Preprocessing and model building (scikit-learn)

Visualization of decision boundaries (ListedColormap)




---

Step 2: Load Dataset

The Iris dataset is read from your Google Drive.

It contains:

An ID column

Four feature columns (sepal/petal length and width)

A target column (Species)




---

 Step 3: Prepare Features and Labels

Features (X): All columns except ID and target.

Labels (y): Only the Species column.

Features are standardized to zero mean and unit variance for better KNN performance.

The target labels (strings like "setosa") are converted into numeric values using LabelEncoder.



---

 Step 4: Train & Evaluate KNN for Different K Values

A range of values for K (from 1 to 10) is tested.

For each value of K:

A KNN classifier is trained on the training data.

The model is evaluated on the test set.

Accuracy is calculated and stored.




---

Step 5: Plot Accuracy vs. K

A line plot is generated showing how model accuracy changes with different values of K.

Helps identify the best K that gives the highest accuracy.



---

Step 6: Select and Train Best KNN Model

The best K (highest accuracy) is selected.

A final KNN model is trained with this optimal K on the training data.

The model predicts the test set.



---

 Step 7: Evaluate with Confusion Matrix

A confusion matrix is generated to show how well the classifier performed:

True positives

False positives

False negatives


The matrix is visualized using a heatmap-style plot.



---

 Step 8: Visualize Decision Boundaries

Only the first two features are used for plotting in 2D.

A mesh grid is created across the feature space.

The KNN classifier predicts class for each point in the grid.

These predictions are plotted as background colors (decision regions).

The actual data points are plotted on top.

A custom legend is created using color patches, mapping each class label to a color.



---
