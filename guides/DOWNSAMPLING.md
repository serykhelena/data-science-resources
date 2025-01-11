# Downsampling 

| <div style="width:500px">NearMiss-1</div> | <div style="width:500px">NearMiss-2</div> |
|-------------------------------------------|-------------------------------------------|
| <div style="width:500px">[NearMiss-1](https://imbalanced-learn.org/stable/under_sampling.html#mathematical-formulation) selects the positive samples for which the average distance to the N closest negative class samples is the smallest.</div>| <div style="width:500px">[NearMiss-2](https://imbalanced-learn.org/stable/under_sampling.html#mathematical-formulation) selects the positive samples for which the average distance to the N farthest negative class samples is the smallest.</div> |

<p float="left">
  <img src="../assets/downsampling/near-miss-1.png" height=500 width="500" />
  <img src="../assets/downsampling/near-miss-2.png" height=500 width="500" /> 
</p>

| <div style="width:500px">ClusterCentroids</div> | <div style="width:500px">Edited Nearest Neighbors</div> |
|-------------------------------------------|-------------------------------------------|
| <div style="width:500px">[The approach](https://imbalanced-learn.org/stable/under_sampling.html#cluster-centroids) makes use of K-means to reduce the number of samples. Therefore, each class will be synthesized with the centroids of the K-means method instead of the original samples</div> | <div style="width:500px">[The approach](https://imbalanced-learn.org/stable/under_sampling.html#edited-nearest-neighbors) applies a nearest-neighbours algorithm and “edits” the dataset by removing samples which do not agree “enough” with their neighbourhood</div> |

<p float="left">
  <img src="../assets/downsampling/cluster-centroid.png" height=315 width=500 />
  <img src="../assets/downsampling/edit-nn.png" height=315 width=500 /> 
</p>

| <div style="width:500px">Instance Hardness Threshold</div> | <div style="width:500px">Neighborhood Cleaning Rule</div> |
|-------------------------------------------|-------------------------------------------|
| <div style="width:500px">[This approach](https://imbalanced-learn.org/stable/under_sampling.html#instance-hardness-threshold) is a specific algorithm in which a classifier is trained on the data and the samples with lower probabilities are removed</div> | <div style="width:500px">[This approach](https://imbalanced-learn.org/stable/under_sampling.html#condensed-nearest-neighbors-and-derived-algorithms) is sensitive to noisy data ⚠️ It focuses on cleaning the data than condensing them. Therefore, it will use the **union** of samples to be rejected between the ENN algorithms and the output of a 3 nearest neighbours classifier.</div> |

<p float="left">
  <img src="../assets/downsampling/instance-ht.png" height=315 width=500 />
  <img src="../assets/downsampling/ncr.png" height=315 width=500 /> 
</p>


