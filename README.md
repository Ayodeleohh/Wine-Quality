# Wine-Quality
Predicting the quality of wine using Decision Trees and Random Forests

Decision Tree

Preprocessing:
To begin working with the decision tree algorithm and wine dataset, I had to import the rpart, rpart.plot, caret and gmodels libraries to create and visualize the tree. 

My next step was data exploration where I explored the wine dataset as shown below. The dataset includes 11 variables that are features of wine quality. 

After looking at the features of the dataset I split my data into training and test sets, and examined the distribution of the quality amongst my new subsets. 

I created the tree below that ranked wines without including the rank variable I created.

Summary: Here it’s visible my tree is split on alcohol, sulphates, and volatile acidity. Higher quality wines tend to have a higher percentage of alcohol and sulphates. The majority of wines in the training set were ranked as 5 or 6, or Okay in terms of my grouped ranking. 

Random Forest

Many of the preprocessing steps were the same to create a random forest model. The classifier has a 43% OOB error rate with 5 trees. With 50 trees the error rate is decreased to just 34%. When increasing the number of trees to 500 I reach an error rate of 32%. 

the error rate plateaus at under 100 trees. After this the accuracy based on the number of trees is less significant. When looking at the error rate at each of my test number of trees, it’s clear that more trees are more effective, to a point. I created a random forest model using all features and got an error rate of 27%. 

Summary:
Using Random forests I was able to achieve a higher accuracy rate than with a single tree alone. There is also the added benefit of knowing which features weigh the most in creating partitions. The error rate I got when using random forests were less than the error rate for a single decision tree.  




