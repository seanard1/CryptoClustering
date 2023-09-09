# CryptoClustering
Module 19 Challenge -- Unsupervised Machine Learning

## Instructions/Premise

In this challenge, you’ll use your knowledge of Python and unsupervised learning to predict if cryptocurrencies are affected by 24-hour or 7-day price changes.

## Modules

warnings

pandas

hvplot.pandas

holoviews

sklearn

## Summary

The Jupyter Notebook `Crypto_Clustering` contains all the relevant code to apply unsupervised machine learning tactics to a CryptCurrent dataset. Running the cells through imports the data, cleans it, scales it and analyzes it in multiple ways to see how different clustering techniques can dial in different results. 

The dataset, in this case, is optimized with four clusters using the K-Means method. This is tested with the Calinski Harabasz scores using Agglomerative and BIRCH for comparison, but K-Means is the best.

There is also a comparison done by using the original dataset and the dataset when scaled down using principal component analysis (PCA). Contrasting these methods shows how PCA can better group the clusters of crytpo when compared to each other. 

## Notes

Some of the starter code from the workbook has been replaced by functions to minimize repetitive code.
Warnings have been supressed for a cleaner presentation.

## Citations

https://stackoverflow.com/questions/69596239/how-to-avoid-memory-leak-when-dealing-with-kmeans-for-example-in-this-code-i-am

- Warning suppression

https://www.w3schools.com/colors/colors_groups.asp

- Originally had the final scatter plots overlayed, but changed that in the end as colours weren't doing enough for visual separation.

## Questions

#### Answer the following question: 

**Question:** What is the best value for `k`?

**Answer:** Arguably, the best cluster value is 4. 

<hr>

#### Answer the following question: 

**Question:** What is the total explained variance of the three principal components?

**Answer:** 89.5%

<hr>

#### Answer the following questions: 

* **Question:** What is the best value for `k` when using the PCA data?

  * **Answer:** Still four.


* **Question:** Does it differ from the best k value found using the original data?

  * **Answer:** It does not.

<hr>

#### Answer the following question: 

  * **Question:** After visually analyzing the cluster analysis results, what is the impact of using fewer features to cluster the data using K-Means?

  * **Answer:** The clusters are a little tighter (less inertia) and easier to visually identify. The original data clusters have more spread and some crossover areas, making interpretation less obvious at a glance. 

