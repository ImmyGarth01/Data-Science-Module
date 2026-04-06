# K-Means Clustering Research Notes

### Video 1 - StatQuest: K-means clustering 
##### Step 1: Identify the number of clusters you want in your data (k = clusters)
##### Step 2: Randomly select distinct data points (the initial clusters)
##### Step 3: Measure the distance between the 1st point and the initial clusters 
##### Step 4: Assign the first point to the nearest cluster and this is how you assign all the datapoints 
##### Step 5: Calcuate the mean of each cluster then measure the cluster using the mean values until it doesn't change 
- K-Means clustering works on the variation on the total variation of the clusters not what looks good to the eye
- In order to figure out the vlaue for K is jsut trying different values (K=1 = worse)
- A graph thtat shows the reduction in variation and number of clusters will show an "elbow plot" this is where the variation doesn't go down as quickly and this point is normally the best K value you can select
- When the data points are not on a number line and on a graph you use the Euclidean distances 
