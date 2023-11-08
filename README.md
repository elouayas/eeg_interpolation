# eeg_interpolation

In this repository, there is the code that allows to learn a spatial graph from a dataset on which we simulate reconstruction problems.
The LearnGraph module resembles a deep torch model with the closed form interpolating in the forward function. Its learning weights is the adjacency matrix of the graph.
To learn, we use classic gradient descent steps. 
In the notebook it's very basic. But in practice you can play with the hyperparameters (LR, number of iterations, number of epochs) or add a scheduler. 
Similarly, in the example there's no validation set, but it's recommanded to add one. Even if it's very difficult to overfit given the small number of parameters!

More code to reproduc the experiments of the paper will be uploaded soon. Feel free to reach me at yassine.el-ouahidi@imt-atlantique.fr if you are interested!
