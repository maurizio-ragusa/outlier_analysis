# outlier_analysis
Outlier analysis on some financial transactions.

This is a little experiment. We have a database of 150000 transactions, and we tried to study the main statistical proprieties of them, in order to spot suspect frauds. The first ideas are very basic, but then we tried to use more powerful methods like Outlier Local Factor (LFO). The basic idea is that, after extrapolating 34 dimensions we consider interesting to measure, we need to spot the outliers in the distribution of points in this 34-dimensional real space. The LFO gives us a notion of density of points, useful to define an "index of outlierness" for each point.

Many developements can be done; first of all, Principal Component Analysis (PCA) should be a great meathod to reduce the dimensionality of the problem. But first of all, the main problem is to find a proper metric to use when we define the notion of "density". Euclidean metric doesn't fit well our demands, and in order to use PCA we need to define an Hilbert metric (that is, we need to define a scalar product, because we have to apply the spectral theorem in the PCA). We'll keep you updated. 
