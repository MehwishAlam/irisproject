# Iris Dataset Exploratory Data Analysis (EDA) and Visualization

This repository contains the Exploratory Data Analysis (EDA) of the Iris dataset, which includes data exploration, visualizations, and some basic preprocessing steps using Python libraries like pandas, seaborn, and matplotlib.

## Dataset Information
The Iris dataset consists of 150 samples from three species of Iris flowers:
Iris-setosa
    
Iris-versicolor
    
Iris-virginica
    

Each sample includes measurements of the following features:


SepalLengthCm
, SepalWidthCm
, PetalLengthCm
, PetalWidthCm

These measurements are used to classify each flower into one of the three species.

## EDA Workflow

### 1. Data Loading:
The dataset is loaded using the pandas.read_csv() method from a CSV file.

### 2. Basic Data Exploration:

    df.head() and df.tail(): Display the first and last few rows of the dataset.
    
    df.info(): Overview of the dataset, including data types and non-null counts.
    
    df.describe(): Summary statistics for numerical features.
    
    df.shape: Shows the dimensions of the dataset.
    
    df.columns: Lists all the column names.

### 3. Data Quality Checks:

    Missing Values: Checked using df.isna().sum(). No missing values are found.
    
    Duplicate Values: Checked using df.duplicated().sum(). No duplicate values are found.
    
    Inconsistent Data: Checked by inspecting the unique values in the target column Species.

### 4. Outlier Detection:

Box Plots: Generated to visualize outliers for each feature with respect to species.

### 5. Target Variable Distribution:

Count Plots: Visualized using sns.countplot() to display the distribution of the three species.
Proportional Representation: The proportion of each species is displayed using value_counts(normalize=True).

### 6. Pairwise Feature Analysis:

Pair Plots: Created using sns.pairplot() to visualize the relationships between the features for different species.

### 7. Correlation Analysis:

Correlation Matrix: Calculated using df.corr() and visualized with a heatmap using sns.heatmap() to show the relationships between features.

### 8. Feature Distributions:

Count Plots: Plots for each feature to visualize their distribution in the dataset.

### 9. Label Encoding:

Label Encoding: The categorical Species column is encoded to numerical values using LabelEncoder from sklearn.preprocessing.

### Visualizations

Several visualizations are included in the analysis:

Box Plots: To observe feature distributions and outliers across species.

Count Plots: To visualize the frequency of each category or feature.

Pair Plots: To display relationships between multiple features and species.

Correlation Heatmap: To highlight correlations between numerical features.

### Requirements
The following Python libraries are used in this project:

pandas
seaborn
matplotlib
sklearn

### Install the required dependencies with:

    pip install pandas seaborn matplotlib scikit-learn
