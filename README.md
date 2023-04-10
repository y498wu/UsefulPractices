# MachineLearningAlgorithms

## SVM
SVMs, support vector machines are a set of **supervised** learning methods used for classification, regression and outlier detection. 

### Linear Kernel
Before:
![Screenshots](screenshots/LinearSVM-before.png)
After:
![Screenshots](screenshots/LinearSVM-after.png)

### RBF (Gaussian Radial Basis Function) kernel 
Before:
![Screenshots](screenshots/RbfSVM-before.png)
After:
![Screenshots](screenshots/RbfSVM-after.png)

### RBF kernel 3D Version
The previous two examples are quite simple and straightforward. It's either linear data (numpy arrays), or sklearn datasets. <br />
I read somewhere that rbf kernel can be quite powerful. Not only I can use it for more complicated dataset, like plotting 3D scatter fig instead of 2D.
For dataset, I download the chess games csv from Kaggle. <br />

![Screenshots](screenshots/Kaggle-Chess-Game.png)

I implemented fitting() function, started by splitting "rating_difference" and "turns" fields (X), and "white_win" (y) dataframes into training and test data. <br />
I use sklearn svm SVC rbf (radial basis function) kernel to train and fit the model. Using this model, I can predict the training and testing X. <br />
Then I generate the ratio of the number of correctly classified samples to the total number of samples, and the classification reports of test and training data. <br />
After fitting() function, I implemented Plot_3D() by visualizing the test data and the svm rbf model's predictions using plotly 3d scatter. <br />

![Screenshots](screenshots/Rbf3DSVM.png)
