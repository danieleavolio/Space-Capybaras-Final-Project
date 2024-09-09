# House Prices Analysis

This project aims to predict the sale price range of houses in Ames, Iowa based on various features about the houses. The dataset used comes from a Kaggle competition called "House Prices: Advanced Regression Techniques".

## Motivation
The goal of this project is to convert the continuous sale price variable into a categorical one with three ranges: low (0-150,000), medium (150,000-300,000), and high (300,000 and above). This is different from the original Kaggle competition, which focused on predicting the exact sale price.

## Approach
We followed the CRISP-DM (Cross-Industry Standard Process for Data Mining) methodology to structure our project. This involved:

1. **Business Understanding**: Defining the problem and objectives.
2. **Data Understanding**: Exploring and analyzing the dataset to gain insights.
3. **Data Preparation**: Cleaning, transforming, and preparing the data for modeling.
4. **Modeling**: Applying various machine learning models to the data, including Decision Trees, Random Forests, Gradient Boosting, AdaBoost, Gaussian Naive Bayes, K-Nearest Neighbors, and Support Vector Classifiers.
5. **Evaluation**: Assessing the performance of the models using metrics like accuracy, precision, recall, and F1-score, as well as techniques like K-fold cross-validation and ROC curves.

## Key Findings
- The Random Forest and Gradient Boosting models consistently outperformed the other models, achieving high accuracy, precision, recall, and F1-scores.
- Handling the class imbalance in the dataset (with the "high" price range having very few instances) was crucial, and we used techniques like SMOTE oversampling to address this.
- Feature selection using techniques like SelectKBest did not lead to significant improvements in model performance, so we opted to use the full set of features.
- Despite trying, we were not able to significantly improve the models' performance through parameter tuning, likely due to the limitations of our computational resources.

## Interesting Insights
- Some features, such as "YearBuilt", showed a strong correlation with the sale price range, indicating their importance in predicting house prices.
- Categorical features like "Alley", "Condition1", and "Condition2" were initially included but ultimately removed, as they did not seem to provide significant predictive power.
- We explored the use of neural networks but found that the other models, such as Random Forest and Gradient Boosting, outperformed them on this dataset.

## Conclusion
This project demonstrates the application of machine learning techniques to the problem of predicting house price ranges. The strong performance of the Random Forest and Gradient Boosting models highlights their effectiveness in capturing the complex relationships between house features and sale prices. The insights gained from this analysis can be useful for real estate professionals, homebuyers, and policymakers in understanding the factors that influence house prices in the Ames, Iowa area.