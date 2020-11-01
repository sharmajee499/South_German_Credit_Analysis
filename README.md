# South_German_Credit_Analysis
Decision Tree Model on imbalanced dataset with various approach.

## Info About Data
The data was extracted from : https://archive.ics.uci.edu/ml/datasets/South+German+Credit.
This is a binary classification problem with the task of classifying good or bad credit. There are about 1000 data points having 19 variable. The dataset is imbalanced. (Good:700, Bad: 300). 

## Purpose

The main purpose of the experiment is to analyze the difference made by the oversampling technique on an imbalanced dataset. 

There are total of 3 model in the notebook.

* Model 1

    - The first model is made up of vanille Decision Tree Model.
    - We were able to get accuracy of 71% however, f1-score was 66%.
    - The AUC was 0.67.
    
 * Model 2
 
    - The second model was hyperparameter tuned (Grid Search) which gave us 67% accuracy, 48% of f1-score and 0.59 AUC.
    - Again, Random Grid Search was implemented which improved the model's accuracy to 73%, f1-score to 56% and AUC to 0.74.
    
 * Model 3
 
    - At, last I used Oversampling method called SMOTE (Synthetic Minority Oversampling Technique) to oversample the minority class.
    - This balanced the two classed(700 each) and increased the total sample to 1400.(1000 at first).
    - Again, the hyperparameter were tuned by Random Search.
    - The accuracy was 74%, f1-score was 74% and AUC was 0.75.
    

## Conclusion

As we can see from above findings that the model's precision and recall (as well as f1) score can be improved on imbalanced data using the oversampling or undersampling methods. (depending upon problem). There hasn't been a drastically improvemet in the accuracy however, the f1-score was significantly improved. Moroever, the performance can be increased by hyperparameter tuning. 
    
 
