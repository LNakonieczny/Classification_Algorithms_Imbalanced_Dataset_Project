# Classification_Algorithms_Imbalanced_Dataset_Project

This project is partially based on the notebook that was created for the peer review assignment in the ‘Machine Learning with Python’
course which is part of the ‘IBM Data Science Professional Certificate’ by IBM available online on Coursera https://www.coursera.org/learn/machine-learning-with-python. <br>

Dataset was prepared by IBM, preliminary data exploration, visualization and preparation steps are based in part on notebook provided
for the course participants and created by Saeed Aghabozorgi, PhD. <br> 


This project contains the following modifications:
- since wget is not available natively on Windows we implemented file download with the urllib.request module,
- we visualized chosen feature before and after use of StandardScaler,
- we used the GridSearchCV for finding hyperparameters for discussed classifiers,
- since provided dataset is unbalanced, we implemented three ways of tackling this problem:
    - use of class_weight feature implemented in all but KNN classifiers to find best algorithm,
    - use resampling method,
    - use of SMOTE (Synthetic Minority Oversampling Technique) from imblearn, <br>
- because main goal of the model is to identify clients that are most likely to defaults on their debt, we choose the F1 score as to score models inside GridSearchCV. Use of the recall leads to the models for which all predictions belong to the majority class.
 
