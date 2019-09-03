# Application ideas of clustering time series

* Just general clustering
* Application to time series classification, maybe develop a framework to use clustering with hidden labels in order to build a cluster based time series classifier. Lots of ideas there
* Note we can do these things on a single time series or on several time series, with different goals.
* Anomaly detection, Local outlier Factor but for time series, isolation forest type models again for time series
* Creating a model which fits stepwise time series models based on the type of model appropriate (thats a time series clustering thing)
* Clustered VAR
* clustered SVAR (structural VAR which is this really cool thing, using structural clustering)
	* SVAR models the data as kind of constant pattern and then it has structural shocks, which we could define at the point of a new cluster or something. I do not know much about this but it might be worth a look.
* Some sort of version of [BSTS](https://en.wikipedia.org/wiki/Bayesian_structural_time_series) for very high dimensional time series, where the features are first clustered and then spoke and slabbed, for massive feature reduction. Instead of several time series we use the centroids of the clusters or something

