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
  5. Compute the new centroid for each of the clusters.<br>
![equation](http://www.sciweavers.org/upload/Tex2Img_1474844222/eqn.png)
* where k is a parameter of the algorithm (the number of clusters to be found), i iterates over the all the intensities,j iterates over all the centroids and µ are the centroid intensities.

## Usage:
<code> usage: kmeans_imgsegment.py [-h] -i SOURCE_IMG -k BIN_SIZE </code>

## Original Image:
![original_img](https://i.imgur.com/TFrg9IZ.jpg)

## Sample Output: 
 * K=2
![k=2](https://i.imgur.com/PHSzSfG.png)
 * K=3
![k=3](https://i.imgur.com/cTc7HIt.png)
 * K=5
![k=5](https://i.imgur.com/qLJcGlC.png)
 * K=8
![k=8](https://i.imgur.com/NbCFqab.png)
 * K=10
![k=10](https://i.imgur.com/CdLEUp5.png)
 
## References: 
  * https://www.ics.uci.edu/~dramanan/teaching/ics273a_winter08/projects/avim_report.pdf
