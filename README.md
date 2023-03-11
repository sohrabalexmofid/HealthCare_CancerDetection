**CancerDetection_ICMR Data**

 *identification of various cancer types based on genes to reduce fatality rate*
 
<p align="center">
  <img width="261" alt="Screenshot 2023-03-10 at 3 20 26 PM" src="https://user-images.githubusercontent.com/123208599/224420946-742b7958-56d4-48d7-a859-ef6224a30cf8.png">
</p>

#




Problem Statement:

ICMR wants to analyze different types of cancers, such as breast cancer, renal cancer, colon cancer, lung cancer, and prostate cancer becoming a cause of worry in recent years. They would like to identify the probable cause of these cancers in terms of genes responsible for each cancer type. This could lead us to early identification of each type of cancer reducing the fatality rate.


***Dimensionality Reduction***:

Each sample has expression values for around 20K genes. However, it may not be necessary to include all 20K genes expression values to analyze each cancer type. Therefore, we will identify a smaller set of attributes which will then be used to fit multiclass classification models. So, the first task targets the dimensionality reduction using various techniques such as,
PCA, LDA, and t-SNE.

Input: Complete dataset including all genes (20531)

Output: Selected Genes from each dimensionality reduction method

***Clustering Genes and Samples***:

Our next goal is to identify groups of genes that behave similarly across samples and identify the distribution of samples corresponding to each cancer type. Therefore, this task focuses on applying various clustering techniques, e.g., k-means, hierarchical and mean shift clustering, on genes and samples.

***Building Classification Model(s) with Feature Selection***:

Our final task is to build a robust classification model(s) for identifying each type of cancer. It also aims at the to do feature selection in order to identify the genes that help in classifying each cancer type.

  classification model(s) using multiclass SVM, Random Forest, and Deep Neural Network to classify the input data into five cancer types
  Validation of the genes selected from the last step using statistical significance testing (t-test for one vs. all and F-test)
