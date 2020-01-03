# Breast-Cancer-Kaggle
During our investigation on Breast Cancer Cell data we have discovered that two groups of cells are responsible for cancerous tumours, those are benign and malignant.

We aimed to discover 1). If characteristics were significantly different between diagnosis groups. 2). Were there any strong associations among the tmour cell characteristics? and 3). Could we predict malignancy of tumours based on characteristics of cell nuclei

After cleaning and transforming the necessary columns of data, our EDA led us to drop more unneccesary features.

We examined features using histrogram plots which suggested cell characteristics were different between diagnosis groups.

We used a Welch's T-Test to measure statistical significance between the means of the two groups for each remaining characteristics all bar one of which were P<0.05.

A correlation matrix Heatmap was employed to identify strong associations between characteristics and those with correlation >0.9 were dropped from the dataset going forward.

Finally we employed an ols regression to measure the model fit using the characteristics we had extracted at this point.

The model output shows R^2 of >0.7, suggesting that we can with 71% accuracy predict the diagnosis of the cell type (malignant of benign) from a set of specific cell characteristics