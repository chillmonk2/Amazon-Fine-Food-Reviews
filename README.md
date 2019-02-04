# Amazon Fine Food Reviews

## t-SNE on dataset:
  ### Conclusion:
  By Observing t-SNE Plots for Bag of Words,TF-IDF,Average W2V and Weighted W2V

  1. We are using first 2500 data points for visualizing the t-SNE plot for above mentioned four techniques.
  2. For Bag of Words visualizing first 2.5k points using t-SNE dense graph with few outliers but distinguishing   with this    diffucult.
  3.Similarly for TF-IDF,Average word to vector and and weighted word to vector we visualized using t-SNE with perplexity is  equal to 30 and learning rate 200. 
  
## Naive Bayes Classification:
  ### Conclusion:
  | Parameter        | Bag of Words         |TF-IDF  |
| ------------- |:-------------:| -----:|
| Alpha     |  0.1  |   0.1 |
| Best AUC Test      | 0.81      |   0.7468 |
|       TN      |    15446     | 16339  |
|       FN      |     966      |  1594  |
|       FP      |     1119     |  226   |
|       TP      |     2269     |  1641  |

