# Iris Dataset: Pattern Recognition System

This project uses the Iris dataset to design and implement a pattern recognition system. The goal is to classify and visualize species patterns using a Decision Tree algorithm. The system involves various stages including data preprocessing, feature analysis, modeling, validation, and visualization.

---

## Project Overview

The Iris dataset is a classic dataset used for machine learning. It contains 150 samples of iris flowers, with 50 samples each from three species:
- Setosa
- Versicolor
- Virginica

Each sample has four features:
- Sepal Length
- Sepal Width
- Petal Length
- Petal Width
The objective is to classify the species based on these features and identify patterns between the features and the species.

---

## Features of the Project
1. Data Preprocessing:
  - Loading the dataset.
  - Encoding categorical target labels.
  - Splitting data into training and testing sets.

2. Feature Analysis:
  - Exploring relationships between features.
  - Visualizing feature distributions and pairwise comparisons.

3. Modeling:
  - Building a Decision Tree classifier.
  - Training the model on the training data.

4. Validation:
  - Evaluating model performance using accuracy and confusion matrix.

5. Visualization:

  - Plotting pairwise relationships between features and species.
  - Visualizing feature-specific patterns (e.g., petal length with species).

---

# Workflow

### 1. Data Preprocessing
- Loading Dataset:
```python
from sklearn.datasets import load_iris
iris = load_iris()
data = pd.DataFrame(data=iris.data, columns=iris.feature_names)
data['species'] = iris.target_names[iris.target]
```
- Label Encoding:
Categorical species labels (e.g., setosa) are converted into numerical labels (e.g., 0, 1, 2) using:
```python
from sklearn.preprocessing import LabelEncoder
label_encoder = LabelEncoder()
y_encoded = label_encoder.fit_transform(data['species'])
```


# Author
Your Name Vaishnavi Pangare
GitHub: https://github.com/Vaishnavi639

# Collaborations
This project is open to collaborations! 


