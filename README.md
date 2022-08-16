<img src="https://bit.ly/2VnXWr2" alt="Ironhack Logo" width="100"/>

# Project 8 - Unsupervised Machine Learning  - 

*Edgar - Mathieu*
*[DA, Paris & 07/22]*

## Description 

In Module 3 we started with a new topic: machine learning unsupervised. The secound week focused on unsupervised learning models and using these to predict and classify given data correctly. The challenge in this weeks project was to use data about the position of cars of uber in New York in April, that inclued the date/time, position of the cars. And create a unsupervised learning model that can determine the clusters of the cars by the position, and try to predict in the future the position of the cars in a certain date/time.

We begn by cleaning and preping the data to be ready for model firring and application. We dealt with transform the Date/Time column that had the type object in to datetime64 type, encode the values of Date/Time in two new columns that contains the day of the weak anda hour, encode the Base column, because the models only acpets columns types integer. Dint deleted outliers, that existed on the position of the cars.

Next step on te way was feature selection for the models and the range of clusters to run the models. Using multiple tests such as Elbow method, NearestNeighbors and Dendrogram. We selected different features being categorized as most important to have the opportunity of testing multiple feature combinations and seeing which will give us the best results from the models.

With all of the necessary information and our cleaned, prepared data we thenn applied following eight supervised learning models.
- KMeans (https://scikit-learn.org/stable/modules/generated/sklearn.cluster.KMeans.html)
		The objective of K-means is simple group similar data points together and discover underlying patterns. To achieve this objective, K-means looks for a fixed number (k) of clusters in a dataset, identifies k number of centroids, and then allocates every data point to the nearest cluster, while keeping the centroids as small as possible.
		K-means algorithm in data mining starts with a first group of randomly selected centroids, which are used as the beginning points for every cluster, and then performs iterative (repetitive) calculations to optimize the positions of the centroids. It halts creating and optimizing clusters when either, the centroids have stabilized, there is no change in their values because the clustering has been successful, and the defined number of iterations has been achieved.

- DBSCAN (https://scikit-learn.org/stable/modules/generated/sklearn.cluster.DBSCAN.html)
		DBSCAN is a density-based clustering algorithm that works on the assumption that clusters are dense regions in space separated by regions of lower density. It groups ‘densely grouped’ data points into a single cluster. It can identify clusters in large spatial datasets by looking at the local density of the data points. The most exciting feature of DBSCAN clustering is that it is robust to outliers. It also does not require the number of clusters to be told beforehand, DBSCAN requires only two parameters: epsilon and minPoints. Epsilon is the radius of the circle to be created around each data point to check the density and minPoints is the minimum number of data points required inside that circle for that data point to be classified as a Core point.

- AgglomerativeClustering (https://scikit-learn.org/stable/modules/generated/sklearn.cluster.AgglomerativeClustering.html)
		The agglomerative clustering is the most common type of hierarchical clustering used to group objects in clusters based on their similarity. It’s also known as AGNES (Agglomerative Nesting). The algorithm starts by treating each object as a singleton cluster. Next, pairs of clusters are successively merged until all clusters have been merged into one big cluster containing all objects. The result is a tree-based representation of the objects, named dendrogram. Agglomerative clustering works in a “bottom-up” manner. That is, each object is initially considered as a single-element cluster (leaf). At each step of the algorithm, the two clusters that are the most similar are combined into a new bigger cluster (nodes). This procedure is iterated until all points are member of just one single big cluster (root) (see figure below).


To recieve the best possible outcome of our model (also regarding the precious business in this case --> importanc of finding the area where the Uber drivers should be to maximize their chances of finding a ride, we tried out different sampling methods to allow the models to perform different classification processes.

## Plan
- Create Trello workflow visualization 
- Create repo on GitHub
- Data cleaning and preparation in jupiter
- EDA and encoding of data
- Sampling data
- Scaler data
- Aplication of Elbow method to define numer of clusters for KMeans
- Aplication of NearestNeighbors to define parameters for DBSCAN
- Aplication of Dendrogram method to define numer of clusters for AgglomerativeClustering
- Application of our models
- Comparaison of our models with Silhoutte Coefficient and Calinski Harabasz
- Comparaison of our models with visualization of clusters on maps
- Fit the best model to data of prediction, and plot for a given day on map
- Prepare presentation

## Deliverables

- Original data in csv format
- Cleaning code
- Clean data in cvv format
- Slides for presentation

## Links to deliverables and additional links

[Repository](https://github.com/Edgart371/Project8)  
[Trello] (https://trello.com/invite/b/kWpE9P3x/b9fa448e759ce3133486cea6e1ecab1d/prj8)





