# Recent Techniques of Clustering Time Series Data: A Survey: Notes

## Abstract: 

* Three types of ts clustering
	* raw data
	* feature based
	* model based
* We will summarize the state of the field as of 2012

## Introduction

> what is time series clustering?

Unsupervised classification of a set of unlabeled time series into groups or clusters, where each group is more or less homogeneous.
 
 Two types of clustering:
 * Shape level:
 	* Based on multiple time series
* Structural level:
	* Based on a single, very long time series 


## Major issues with time series clustering:

* High dimensionality
* Temporal order issues
* Noise

## Three types again:

1. Temporal-Proximity-Based Clustering:
	* Works directly on raw data, either in frequency or time domain
2. Representation-Based Clustering:
	* Works indirectly with features extracted from the raw data
3. Model-Based Clustering:
	* Works on the models built from the raw data (pretty wild)


## Making an effective model;

There are two techniques for making an effective time series clustering model:

1. Representation methods
	* Discrete Fourier Transform
	* Single Value Decompostion
	* Discrete Cosine Transformation
	* Discrete Wavelet Transformation
	* Piecewise Aggregation
	* etc.
	* There are a lot of these
	* These reduce the dimensionality of the series
2. Distance Measued
	* At least 12 of these
	* Cool things like DTW, ED, LCSS, DISSIM, SpADe etc.


# Temporal-Proximity Clustering

This useually works with raw data

* The big point of contention here is the distance/similarity measure for time series data


[Kumar](KumarSeasonalPatterns.pdf): Distance function based on independent models of data errors and clustered hierarchically, grouping time series into seasonal sequences with a good number of clusters. Data must be preprocessed to remove nonseasonal factors and nomralized.

[Liao(1)](Liao-TwoSteps.pdf): Two step procedure for clustering multivariate time series of equal or unequal or unequal length:
	1. k-means or fuzzy c-means(FCM) to time stripped data, in order to convert it into a univariate series with discrete values. The times are then added back in to the dataset, making it a time series again. 
	2. On the converted variable, employ k means or FCM to group the converted time series, expressed essentially as probability matrices into clusters. Euclidean distances are used in step one, where various distance measures are used in step 2

[Liao(2)](LiaoBattle.pdf)
