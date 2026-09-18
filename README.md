# Mammographic Mass Classification

A Python machine-learning project comparing multiple supervised learning techniques for predicting whether a mammographic mass is benign or malignant.

## Project Overview

This project uses the **Mammographic Mass** dataset from the UCI Machine Learning Repository to explore whether characteristics recorded during mammographic assessment can be used to classify a mass as benign or malignant.

The dataset contains 961 cases and includes patient age and characteristics of the detected mass, including its shape, margin and density. The target variable identifies the mass as benign or malignant.

The project covers the process from initial data exploration and cleaning through feature preparation, model training, cross-validation and comparison of several machine-learning approaches.

## Dataset

The original dataset contains the following fields:

* **BI-RADS assessment** — radiological assessment category
* **Age** — patient age in years
* **Shape** — classification of the mass as round, oval, lobular or irregular
* **Margin** — characteristics of the mass boundary
* **Density** — mass density classification
* **Severity** — benign or malignant diagnosis

BI-RADS is excluded as a predictive feature. The models use age, shape, margin and density to predict severity.

The dataset contains missing values, making data cleaning and examination of missing-data patterns an important part of the project.

## What the Project Does

The Jupyter notebook:

* Loads and explores the mammographic-mass dataset using pandas
* Identifies and investigates missing values
* Cleans the dataset for machine-learning analysis
* Examines relationships within the data through visualization
* Selects features for predicting benign versus malignant masses
* Applies feature scaling where appropriate
* Splits data into training and test sets
* Uses cross-validation to evaluate model performance
* Compares several supervised machine-learning algorithms
* Experiments with model parameters and different SVM kernels
* Builds and evaluates a neural-network classifier using TensorFlow/Keras

## Machine-Learning Models Explored

The project applies and compares:

* Decision Tree
* Random Forest
* K-Nearest Neighbors (KNN)
* Multinomial Naive Bayes
* Support Vector Machine (SVM)
* Logistic Regression
* TensorFlow/Keras neural network

Different preprocessing and evaluation approaches are explored, including standardization, MinMax scaling, train/test splitting and K-fold cross-validation.

## Technologies Used

* **Python**
* **pandas** — data loading, cleaning and manipulation
* **NumPy** — numerical operations
* **scikit-learn** — preprocessing, classification and model evaluation
* **TensorFlow / Keras** — neural-network modeling
* **Matplotlib** — visualization
* **seaborn** — statistical visualization
* **pydotplus** — decision-tree visualization
* **Jupyter Notebook** — analysis and documentation

## Repository Contents

`BreastCancerMassImages_DataScienceFinalProject.ipynb`
The Jupyter notebook containing the complete analysis and machine-learning workflow.

## Running the Project

Clone the repository:

```bash
git clone https://github.com/EnragedSpark596/Breast-cancer-screening.git
cd Breast-cancer-screening
```

Install the required Python packages:

```bash
pip install -r requirements.txt
```

Then launch Jupyter:

```bash
jupyter notebook
```

and open:

```text
BreastCancerMassImages_DataScienceFinalProject.ipynb
```

**Data Files**

The repository includes the original UCI Mammographic Mass dataset files used by the notebook:

mammographic_masses.data.txt — the dataset containing the mammographic mass observations used in the analysis
mammographic_masses.names.txt — the accompanying dataset documentation describing the attributes and source data

## Project Context

This is an earlier machine-learning project completed as part of my Python and data-science training and is preserved substantially in its original form as part of my development portfolio.

The project gave me practical experience with several important parts of a machine-learning workflow: inspecting imperfect real-world data, investigating missing values, preparing features, scaling data, training multiple classification algorithms and comparing their performance using cross-validation.

It also provided an opportunity to compare traditional machine-learning methods with a neural-network approach using TensorFlow/Keras.

The notebook uses some APIs from older versions of scikit-learn and TensorFlow/Keras. It therefore represents the Python ecosystem in which the project was originally developed rather than current production code.

## Important Note

This is an educational data-science project and is **not a medical diagnostic tool**. Its models and results should not be used to make clinical or healthcare decisions.

## Data Source

The project uses the **Mammographic Mass** dataset originally published through the UCI Machine Learning Repository.

## Author

**Ian Jones**

Former chemical and process safety engineer developing Python skills in data analysis, automation, machine learning, visualization and practical problem-solving.
