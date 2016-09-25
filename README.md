# Kmeans-Image-Segmentation
##Algorithm Overview: 
- The KMeans algorithm is an unsupervised clustering algorithm that classifies the input data
points into multiple classes based on their inherent distance from each other. The algorithm
assumes that the data features form a vector space and tries to find natural clustering in
them. 
- The points are clustered around centroids ![equation](http://www.sciweavers.org/upload/Tex2Img_1474841178/eqn.png) The algorithm takes a 2 dimensional image as input. 
- Various steps in the algorithm are as follows: 
  1. Compute the intensity distribution(also called the histogram) of the intensities.
  2. Initialize the centroids with k random intensities
  3. Repeat the following steps until the cluster labels of the image does not change anymore.
  4. Cluster the points based on distance of their intensities from the centroid intensities. 
![equation](http://www.sciweavers.org/upload/Tex2Img_1474843269/eqn.png)
  5. Compute the new centroid for each of the clusters.
![equation](http://www.sciweavers.org/upload/Tex2Img_1474844222/eqn.png)
where k is a parameter of the algorithm (the number of clusters to be found), i iterates over the all the intensities,j iterates over all the centroids and µ are the centroid intensities
