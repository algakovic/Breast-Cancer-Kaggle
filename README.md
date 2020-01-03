# Breast-Cancer-Kaggle Project
We conducted an investigation on Breast Cancer Cell Data from Kaggle Breast Cancer Wisconsin Data set:https://www.kaggle.com/uciml/breast-cancer-wisconsin-data 

The data clearly identifies two types of diagnosed cancer tumour cells. Those are benign and malignant.

We aimed to discover 1). If there were strong associations among the tumour cell nuclei characteristics 2). If characteristics were significantly different between diagnosis groups and 3). Could we predict malignancy of tumours based on characteristics of the cell nuclei.

After cleaning and transforming the necessary columns of data, our EDA led us to drop more unneccesary features.

We examined features using histrogram plots which suggested cell characteristics were different between diagnosis groups.

We used a Welch's T-Test to measure statistical significance between the means of the two groups for each remaining characteristics all bar one of which were P<0.05.

A correlation matrix Heatmap was employed to identify strong associations between characteristics and those with correlation >0.9 were dropped from the dataset going forward.

Finally we employed an ols regression to measure the model fit using the characteristics we had extracted at this point.

The model output shows R^2 of >0.717, suggesting that we can with 71% accuracy predict the diagnosis of the cell type (malignant of benign) from a set of specific cell characteristics

Presentation Google slides link: https://docs.google.com/presentation/d/1QFwmSnX6ZeGHmyoZ5S5JWPtKWLS-SWldB6ZukOQZBhM/edit?ts=5e0e263d#slide=id.g76375d83e3_0_67
