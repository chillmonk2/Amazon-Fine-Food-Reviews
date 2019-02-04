# Amazon Fine Food Reviews

## t-SNE on dataset:
  ### Conclusion:
  By Observing t-SNE Plots for Bag of Words,TF-IDF,Average W2V and Weighted W2V

  1. We are using first 2500 data points for visualizing the t-SNE plot for above mentioned four techniques.
  2. For Bag of Words visualizing first 2.5k points using t-SNE dense graph with few outliers but distinguishing   with this    diffucult.
  3.Similarly for TF-IDF,Average word to vector and and weighted word to vector we visualized using t-SNE with perplexity is  equal to 30 and learning rate 200. 
  
## Naive Bayes Classification:

For Naive bayes classification used MultinomialNB because the the multinomial Naive Bayes classifier is suitable for classification with discrete features (e.g., word counts for text classification).The model is trained on value of alpha in the set [0.00001,0.0001,0.001,0.01,0.1,1,10,100]. We find that for both the Bag of Words and TF-IDF the best alpha is 0.1.

  ### Conclusion:
  | Parameter        | Bag of Words         |TF-IDF  |
| ------------- |:-------------:| -----:|
| Alpha     |  0.1  |   0.1 |
| Best AUC Test      | 0.81      |   0.7468 |
|       TN      |    15446     | 16339  |
|       FN      |     966      |  1594  |
|       FP      |     1119     |  226   |
|       TP      |     2269     |  1641  |


## K Nearest Neighbor Classification:

Used 40000 datapoints for the train and testing split.The model is trained on k = [3,5,7,9,11,13,15,17,19,21] for both the version of KNN Algorithm i.e "Brute Force" and "KD Tree". For each of them plotted confusion matrix for best k which is decided from the AUC Score.Please note that the dataset is imbalanced that is why K is decided from the AUC score on cross validated data

  ### Conclusion


  | Parameter        | Bag of Words         |TF-IDF  | Avg W2V | W W2V|
| ------------- |:-------------:| -----:|:-------------:| -----:|
|  Brute Force best K  |      21      |   5    |    21   |   19   |
| Brute Force best AUC |    0.6666    | 0.512  |  0.8763 | 0.847  |
|    Brute Force TN    |    12949     | 13324  |  10802  | 10830  |
|    Brute Force FN    |     2230     |  2595  |   1451  |  1560  |
|    Brute Force FP    |     478      |   63   |   240   |  212   |
|    Brute Force TP    |     383      |   18   |   707   |  598   |
|    KD Tree best K    |      13      |   3    |    21   |   21   |
|   KD Tree best AUC   |    0.7292    | 0.5798 |  0.8762 | 0.8496 |
|      KD Tree TN      |    10489     | 10584  |  10802  | 10829  |
|      KD Tree FN      |     1616     |  1895  |   1451  |  1578  |
|      KD Tree FP      |     553      |  458   |   240   |  213   |
|      KD Tree TP      |     542      |  263   |   707   |  580   |
