I have developed a Bayesian Logistic Regression model as well as a Generative classifier from scratch in numpy. **No ML Libraries (Pytorch/Tensorflow/Scikit-learn) were used**   
I first trained using maximum likelihood then introduced a prior over my weights. I assumed that each weight is independent and identically distributed. Each weight prior was gaussian with a zero mean and diagonal covariance matrix. I used the Laplace approximation to estimate my posterior distribution. Training was done using damped iteratively reweighted least squares  
Then I trained a multi-class generative classifier using maximum likelihood. I assumed that the class conditional densities were gaussian with a shared covariance matrix. Predictions were evaluated using Bayes theorem with MLE estimates.  
The dataset used: https://archive.ics.uci.edu/dataset/602/dry+bean+dataset  
**I have derived all the required equations in my notebook**
