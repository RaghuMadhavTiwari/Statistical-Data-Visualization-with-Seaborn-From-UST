# Statistical-Data-Visualization-with-Seaborn-From-UST

![image](https://user-images.githubusercontent.com/65697330/145578893-2619391f-27dd-4837-93f5-efeb37047bc3.png)

1. Employed the statistical data visualization library, Seaborn, to discover and explore the relationships in the Breast Cancer Wisconsin (Diagnostic) data set. 
2. Perform exploratory data analysis (EDA) on the Breast Cancer Diagnosis, drop correlated features, implement feature selection and utilize several feature extraction methods including; feature selection with correlation, univariate feature selection, recursive feature elimination, principal component analysis (PCA) and tree based feature selection methods. 
3. Lastly, built a boosted decision tree classifier with XGBoost to classify tumors as either malignant or benign. 

**About the Dataset:**
The [Breast Cancer Diagnostic](https://archive.ics.uci.edu/ml/datasets/Breast+Cancer+Wisconsin+%28Diagnostic%29) data is available on the UCI Machine Learning Repository.

Features are computed from a digitized image of a fine needle aspirate (FNA) of a breast mass. They describe characteristics of the cell nuclei present in the image. n the 3-dimensional space is that described in: [K. P. Bennett and O. L. Mangasarian: "Robust Linear Programming Discrimination of Two Linearly Inseparable Sets", Optimization Methods and Software 1, 1992, 23-34].

**Attribute Information:**
1) ID number 2) Diagnosis (M = malignant, B = benign)

Ten real-valued features are computed for each cell nucleus:

a) radius (mean of distances from center to points on the perimeter)
b) texture (standard deviation of gray-scale values)
c) perimeter
d) area
e) smoothness (local variation in radius lengths)
f) compactness (perimeter^2 / area - 1.0)
g) concavity (severity of concave portions of the contour)
h) concave points (number of concave portions of the contour)
i) symmetry
j) fractal dimension ("coastline approximation" - 1)

### The hands on project on Statistical Data Visualization with Seaborn is divided into the following tasks:

**Task 1: Importing Libraries and Data**
- In this task, we will briefly recap our exploratory data analysis of the Breast Cancer Wisconsin (Diagnostic) Data Set from Breast Cancer Diagnosis – Exploratory Data Analysis

**Task 2: Dropping Correlated Columns from Feature List**
- Using the heatmap of the correlation matrix, we were able to identify columns to be dropped. 
- Out of a set of correlated features, we will preserve the one that best separates the data. 
- We will identify these salient features using the violin plots and swarm plots produced in the previous project. 

**Task 3: Classification using XGBoost (minimal feature selection)**
- Drop 15 columns that are correlated out of a total of 33 columns. 
- To verify that there are no remaining correlated features, plot another correlation matrix and inspect the Pearson correlation coefficient. 
- Next, use a helper function from scikit-learn to create split the data into training and test sets. 
- Using the default parameters, fit the XGBClassifier estimator to the training set and use the model to predict values in the test set.   
- Evaluate the performance of the classifier using the accuracy score, f-1 score, and confusion matrix from sklearn.metrics. 

**Task 4: Univariate Feature Selection**
- In univariate feature selection, we will use the SelectKBest() function from scikit-learn. The score returned can be used to select  n features with the highest values for the test chi-squared statistic from the data. 
- Recall that the chi-square test measures the dependence between stochastic variables. 
- Using this function weeds out the features that are the most likely to be independent of class and therefore irrelevant for classification.

**Task 5: Recursive Feature Elimination with Cross-Validation**
- In this task, we will not only find the best features but also the optimal number of features needed for the best classification accuracy.

**Task 6: Plot CV Scores vs Number of Features Selected**
- Evaluate the the optimal number of features needed for the highest classification accuracy by plotting the cross validation (CV) scores of the selected features on the y-axis, against the number of selected features on the x-axis. 

**Task 7: Feature Extraction using Principal Component Analysis**
- Use principle component analysis (PCA) for feature extraction. 
- We will first need to normalize the data for better performance.   
- A plot of the cumulative explained variance against the number of components gives the percentage of variance explained by each of the selected components. This curve quantifies how much of the total variance is contained within the first N components.

What I learnt from this Project-
By the end of this Project, I felt more confident about working with data, creating visualizations for data analysis, and have practiced several methods which apply to a Data Scientist’s role. 

This is a (Guided Project by Coursera)[https://www.coursera.org/learn/statistical-data-visualization-seaborn-ust/home/welcome]
