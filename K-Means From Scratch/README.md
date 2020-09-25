# K-Means

##Steps:

* Load the image apply preprocessing if any required.
* Chosse k points randomly know as means.
* Define number of iterations you want to perform.
* Randomly select K featuresets to start as your centroids.
* For each data point, compute the euclidian distance from all the centroids (2 in our case) and assign the cluster based on the minimum distance to all the centroids.
* Take mean of each class (mean of all featuresets by class), making that mean the new centroid.
