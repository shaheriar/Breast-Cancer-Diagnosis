# Breast Cancer Diagnosis
Using different Machine Learning techniques such as Random Forest Classifier, SVM, and K Nearest Neighbors to predict whether a breast cancer diagnosis is benign or malignant.

# Contributors
<a href="https://github.com/MdAfraaz" target="_blank"><img src="https://avatars.githubusercontent.com/u/59735500?v=4" align="left" height="30px">Afraaz Mohammed</a>

<a href="https://github.com/devbydan" target="_blank"><img src="https://avatars.githubusercontent.com/u/43690299?v=4" align="left" height="30px">Daniel Murphy</a>

<a href="https://github.com/shaheriar" target="_blank"><img src="https://avatars.githubusercontent.com/u/49822364?v=4" align="left" height="30px">Shaheriar Malik</a>

# The Question
This report outlines the findings of the Breast Cancer Diagnosis Classifier data analysis given a set of unique features. Said features will help determine whether the breast cancer is benign or malignant and we will analyze potential factors that may make one prone to having breast cancer.

So, the primary objectives are to answer the following questions:

1) **What factors determine the diagnosis of breast cancer?**

2) **Can Machine Learning be used to diagnose breast cancer?**

# The Data

The dataset can be found [here](https://archive.ics.uci.edu/ml/datasets/breast+cancer+wisconsin+(diagnostic)) through UCI's Machine Learning Repository.

There are two attributes within the dataset:
- [Patient] ID Number
- Diagnosis (M = malignant, B = benign)

and a total of ten features as follows (Each feature includes the mean, standard error and worst case data):
- Radius (mean of distances from center to points on the perimeter) 
- Texture (standard deviation of gray-scale values) 
- Perimeter 
- Area 
- Smoothness (local variation in radius lengths) 
- Compactness (perimeter^2 / area - 1.0) 
- Concavity (severity of concave portions of the contour) 
- Concave points (number of concave portions of the contour) 
- Symmetry 
- Fractal dimension ("coastline approximation" - 1)

# The Approach
Once the data was cleaned, we analyze it to find the most useful features for classification. Once this has been performed, the resultant features will be passed into RandomForestClassifier. The model uses the selected numerical columns to ensure the highest accuracy possible with the given data set.

# Our hypothesis
Without any formal medical knowledge or exposure, we claim that without most of the given features the model can still perform well as most of them are correlated.

# Why Bother?
Having no medical knowledge, teaching a machine to diagnose the chances of breast cancer seems fascinating. Identifying which features matter more for this problem is very useful. If the evaluated metrics are above the rate of human error, this can be used for actual diagnosis.
