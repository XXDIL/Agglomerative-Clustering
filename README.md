# Agglomerative-Clustering
This is based on iteratively finding the distance between the components of the sample at each step and finding a cluster with respect to some linkage criterion till we are able to put the entire sample available in some hierarchy.

# Agglomerative and Divisive Hierarchical CLustering

Course Assignment for IDAA - Machine Learning @ IIIT Allahabad.

**Done under the guidance of Dr. Mohammed Javed, Assistant Professor, IIIT Allahabad**

## Table of contents
- [Introduction](#introduction)
- [Data](#data)
- [Instructions to run the scripts](#instructions-to-run-the-scripts)
- [Equations used](#equations-used)
- [Posteriori Analysis](#posteriori-analysis)
  * [Agglomerative](#agglomerative)
- [Group Members](#group-members)


## Introduction
Hierarchical clustering is a method of cluster analysis which seeks to build a hierarchy of clusters. Strategies for hierarchical clustering generally fall into two types:

1. **Agglomerative**: This is a "bottom up" approach: each observation starts in its own cluster, and pairs of clusters are merged as one moves up the hierarchy.

2. **Divisive**: This is a "top down" approach: all observations start in one cluster, and splits are performed recursively as one moves down the hierarchy.

In general, the merges and splits are determined in a greedy manner. The results of hierarchical clustering are usually presented in a dendrogram.


**The main purpose of this project is to get an in depth understanding of how the Agglomerative and Divisive hierarchical clustering algorithms work.**

*More on [Hierarchical clustering](https://medium.com/@darkprogrammerpb/agglomerative-hierarchial-clustering-from-scratch-ec50e14c3826)*

## Data
We used the random data, the dataset can contains **2 points**.

## Instructions to run the scripts
Run the following command:

##### Agglomerative clustering
```console
foo@bar:~$ python AgglomerativeClustering.py
```

## Equations used
```
Maximum or complete-linkage clustering -> Max(d(a,b))
Minimum or single-linkage clustering -> Min(d(a,b))
Mean or average linkage clustering -> sum of all d(a,b)/(|A|+|B|)
```
*where x, y are points in the same cluster and, a belongs to A, b belongs to B.*

## Posteriori Analysis

![Grapg 1](https://user-images.githubusercontent.com/66634743/84398750-62c94300-ac11-11ea-8f05-9e19cc853d21.png)

##### In the above graph, we notice that the graph takes the form of O( n^3 ).

### Agglomerative
##### CLustering was performed using the agglomerative and divisive methods and the following dendrograms were obtained-

![Agglomerative-Centroid](https://user-images.githubusercontent.com/66634743/84398757-64930680-ac11-11ea-848c-6a2e7ce36dda.png)


## Group Members
Shubham Soni

[Manav Agrawal](http://github.com/mka2011)

[Mohammed Aadil](http://github.com/XXDIL)
