# da-crytoclustering
An unsupervised ML clustering problem relating to cryptocurrency.  
Note: this is a school project. No real insight can be gained from these projections.  

# How to Use

Open the Jupyter Notebook and run all cells.  
Make sure the environment has all of the packages used in the notebook.  

# About the Project

In this project, I use SKLearn's KMeans algorithm to cluster crytocurrency data.
After initial loading of the data, I use SKLearn's StandardScalar to scale the data.

The first KMeans attempt is done with the raw data.  
I generate 11 different projections for an elbow graph to decide the amount of clusters to be used.  
From the graph, I find that 4 clsuters appears to fit the data best.  
After deciding the amount of clusters, I run the projections for 4 clusters and plot the results.  

For the second KMeans attempt, I use PCA to remove issues with collinearity and reduce the dimensions of the dataset.  

Note: the instruction for the PCA dimensions was to use 3 dimensions.  
Without this instruction, I would have kept the same amount of dimensions and reduced based on the explained variance of each component.  

After running PCA and getting the new dataset, it is the same process as above for the graph.  
I run the steps to generate an elbow plot, and then still find that the ideal amount of clusters is 4.  
Then, I run the projections with 4 clusters and plot that graph.  

At the end, there is a comparison of the two elbow plots and two scatter plots.

# Built In

Python.  
Jupyter Notebook.  
