# Model-Selection-of-Clustering
This is a coursework deliverd by University of Glasgow, Machine Learning & Artificial Intelligence for Data Scientists.
And was completed in a group with Weijian Ning.

## Model selection for Clustering
Clustering is unsupervised learning: the resulting clusters are completely derived from data distributed in given a feature set with no class available

Compared to supervised learning counterparts, it is ...
*hard to define model performance (cluster quality)
*sensitive to different clustering algorithms and different feature spaces.

## Task
We try different clustering algorithms and also a range of the potential parameter(s) which affect the number of clusters including ..

* K-means
<https://scikit-learn.org/stable/modules/generated/sklearn.cluster.KMeans.html>

* Hierarchical Clustering
<https://scikit-learn.org/stable/modules/generated/sklearn.cluster.AgglomerativeClustering.html#sklearn.cluster.AgglomerativeClustering>

* HDBSCAN
<https://hdbscan.readthedocs.io/en/latest/basic_hdbscan.html>

on 5K colorectal patches represented by 4 different representation PathologyGAN, ResNet50, InceptionV3 and VGG16

## Data and its preprocessing
5,000 non-overlapping image patches from hematoxylin & eosin (H&E) stained histological images of human colorectal cancer (CRC) and normal tissue.

* 4 feature sets, PathologyGAN, ResNet50, InceptionV3 and VGG16, are extracted to represent those 5,000 images different dimensional feature spaces.

* PCA and UMAP were employed to reduce each feature sapce into 100-dimensional vectors

* 9 tissue types are also available which include Adipose (ADI), background (BACK), debris (DEB), lymphocytes (LYM), mucus (MUC), smooth muscle (MUS), normal colon mucosa (NORM), cancer-associated stroma (STR), colorectal adenocarcinoma epithelium (TUM)

## Performance Measurement
To assess quality of clustering solutions, several approaches are expected to be done and interpreted which include...

* Silhouette Score for goodness of fit test
* Vmeasure Score for homogeneity and completeness test (tissue type available as ground truth)
* Adjust Rand Index
* Clusters visualisations

For more the final report, please have a check in the .pdf file.
