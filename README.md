# Adult-Data-Classification

This was created in collaboration with Andreea Al-Afuni

Readme for better understanding of the Jupyter notebook:

Used libraries:
- mathplotlib
- numpy
- pandas
- sklearn
- scipy
- seaborn
- math

The most extensively used library was sklearn. The used parts include:
- preprocessing (for different scalers, e.g. StandardScaler, RobustScaler, …)
- model_selection (for train_test_split)
- metrics (for evaluation
- manifold (for TSNE)

Pandas and numpy were used for storing the dataset as well as locating data and performing some mathematical operations. Seaborn and Mathplotlib were used for many of the plots. 

The notebook is supposed to run in one go. All cells are constructed in a way that information required in a cell should be computed in a previous cell. The order of cells deviates slightly from the order in the project description. There are three main blocks: pre-processing and the two algorithms.
For each algorithm the order of operations is as follows:
1. Testing of different parameters on performance
2. Using the best performing version of the model to predict the new instances in the test set
3. More in depth evaluation of the model (e.g., external and internal measures)
4. Protected attributes

Although the resulting clusters are mostly consistent between runs, the labels change occasionally (even when a random_state is set). Therefore, in the evaluation of the kMeans algorithm, the cluster labels are swapped in one cell. If the score is below 0.5, this and all subsequent cells have to be run again for accurate results.
