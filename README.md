# Bayesian-Optimization-for-Classifier-Evasion
This code is the implementation of the paper: https://arxiv.org/pdf/1712.08713.pdf. This code is modified based on the Bayesian Optimization code from https://bitbucket.org/woalsdnd/highdim_bo.  

# To run this code: 
1. Execute "experiment_schedule.m" file. This code provides the attack to Linear SVM, RBF kernel SVM and MLP. You are also free to train your own model and apply Bayesian optimization method to attack the underlying classifier. 
2. To switch from SVM to MLP, simply call the function **run_experiment2_diff_C**, Linear SVM and Kernel SVM can be switched inside function "run_experiment1_diff_C".
3. A rough structure of the code is as follows: `experiment_schedule.m` -> `run_experiment1_diff_C.m` -> `BayesianOptimization.m`. `BayesianOptimization.m` is the main part where Bayesian Optimization method is implemented.  

# Results
You should expect to obtain the plot of query number with different feature modification cost *C*.  

# Pre-requisites
You will need Matlab to run the whole code. Training data for the trained model in the paper is preprocessed and is ready in the folder "/Data". To train your own model on your own data, you will need to place the processed data into the "/Data" folder.  
