# K-Means-Clustering-Hierarchical-Clustering-and-DBSCAN-on-Amazon-Fine-Food-Reviews-Dataset

Unsupervised Learning is a Type of Machine Learning Algorithm used to draw Inferences from Datasets consisting of input Data without labeled responses. The most common Unsupervised Learning method is Cluster Analysis, which is used for Exploratory Data Analysis to find hidden patterns or grouping in data. In other words, cluster analysis or clustering is the task of grouping a set of objects in such a way that objects in the same group (called a cluster) are more similar (in some sense) to each other than to those in other groups (clusters).

## Types of Clustering :

1.K-Means clustering

2.Hierarchical Clustering

3.DBSCAN(Density Based spatial clustering of application with noise).

Procedure Followed:

## 1.K-Means Clustering:

• Step1: Take Reviews data of Amazon Reviews data-set. And Ignore score column

• Step2: Apply K-means++ cluster and K-medoids cluster Algorithm.

• Step3: Apply Feature generation techniques(Bow,tfidf,avg w2v,tfidfw2v)

• Step4: Apply K-Means clustering Algorithm using each technique.

• Step5: To find Best k using Elbow method

• Step6: Read the Cluster Reviews

## 2.Hierarchical Clustering:

• Step1: Take 5k Reviews sample of Amazon Reviews data-set. And Ignore Score column

• Step2: Apply Feature generation techniques(Bow,tfidf,avg w2v,tfidfw2v)

• Step3: Apply Hierarchical Clustering Algorithm using each Technique.

• Step4: To find Best k using Elbow method

• Step5: Read the Cluster Reviews

## 3.DBSCAN Clustering:

• Step1: Take sample of Reviews data of Amazon Reviews dataset. And Ignore Score column

• Step2:consider min_pts = 2* dimension(consider 100 dimensions of data).

• Step3: Apply Feature generation techniques(avg w2v,tfidfw2v) BOW & TFIDF is high dimesional thus DBSCAn does not work properly

• Step4: Apply DBSCAN Algorithm using avg w2v & tfidfw2v technique.

• Step5: To find Best k using Elbow method

• Step6: Read the Cluster Reviews

• Step7: As DBSCAN is sensible towards eps value,check the sensitives for different value of eps

## 4. Comparison between K-Means Algorithm and DBSCAN Algorithm

## DBSCAN's Advantages Compared to K-Means:

1. DBSCAN does not require pre-specified input of the number of cluster while K-Means does.
2. DBSCAN can find arbitrarily shaped clusters, while k-means algorithm is good in capturing structure of the data if clusters have a spherical-like shape.
3. DBSCAN has a notion of noise, and is robust to outliers.

## DBSCAN's Disadvantages Compared to K-Means:

1. The performance of DBSCAN depends heavily on the parameter values.
2. DBSCAN cannot cluster data sets well with large differences in densities, since the minPts-epsilon combination cannot then be chosen appropriately for all clusters.
3. DBSCAN is not entirely deterministic: border points that are reachable from more than one cluster can be part of either cluster, depending on the order the data are processed.
4. Like K-means, DBSCAN is scalable, but using it on very large datasets requires more memory and computing power.
