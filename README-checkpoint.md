# Machine Learning Project: How to predict the audience of TV Globo productions?  
---
### The project uses a dataset with information about Rede Globo TV productions that aired between 1965 and 2018.  
### The objective of the project is to predict the audience of the productions using the information obtained through the features.   
---
#### The following treatment was done in the dataset:  
1. The columns ['Start','End','Novel','Range','Biggest','Most Famous','Rating','Menu'] that were not needed for the analysis were deleted.  
2. "Dummies" from the pandas library were used to suppress the "Autor" column and insert new columns with numerical values in its place.  
3. As target "y", the "Audiencia" column was chosen, which is what you want to predict. All columns that remained in the dataset after treatment were chosen as "X" features, except for the "Audiencia" column.  
4. The dataset was divided into 4 parts to carry out the training and tests: train_X, val_X, train_y, val_y  
5. The method chosen for the model was DecisionTreeRegressor because it achieved the best result in the r2_score score.  
6. The other methods tested that obtained a lower result were the regressions: Linear, Ridge and Lasso.   
---
### **Conclusion:**  
1. Using the generated model, the following result was found through r2_score: 0.697070598916826.  
2. This means that the prediction obtained a successful result, even if some deviations were found.  
3. It was possible to find some values very close to the real values expected for the audience of Rede Globo TV productions.  