# MachineLearningAlgorithms

## SVM
SVMs, support vector machines are a set of **supervised** learning methods used for classification, regression and outlier detection. 

### Linear Kernel
Before:
<br />
![Screenshots](screenshots/LinearSVM-before.png)
<br /><br />
After:
<br />
![Screenshots](screenshots/LinearSVM-after.png)

### RBF (Gaussian Radial Basis Function) kernel 
Before:
<br />
![Screenshots](screenshots/RbfSVM-before.png)
<br /><br />
After:
<br />
![Screenshots](screenshots/RbfSVM-after.png)
<br />
Reference: <br />
[Linear and RBF Kernel SVM Tutorial](https://www.freecodecamp.org/news/svm-machine-learning-tutorial-what-is-the-support-vector-machine-algorithm-explained-with-code-examples)
<br />

### RBF kernel 3D Version
The previous two examples are quite simple and straightforward. It's either linear data (numpy arrays), or sklearn datasets. <br />
I read somewhere that rbf kernel can be quite powerful. Not only I can use it for more complicated dataset, like plotting 3D scatter fig instead of 2D.
For dataset, I download the chess games csv from Kaggle. <br />

![Screenshots](screenshots/Kaggle-Chess-Game.png)

I implemented fitting() function, started by splitting "rating_difference" and "turns" fields (X), and "white_win" (y) dataframes into training and test data. <br />
I use sklearn svm SVC rbf (radial basis function) kernel to train and fit the model. Using this model, I can predict the training and testing X. <br />
Then I generate the ratio of the number of correctly classified samples to the total number of samples, and the classification reports of test and training data. <br />
After fitting() function, I implemented Plot_3D() by visualizing the test data and the svm rbf model's predictions using plotly 3d scatter. <br />
From the screnshot, we can see that the black dots on top are the cases when white wins. The surface in the middle is the dicision boundary set by the rbf kernel model. The black dots at the botton are the cases when white doesn't win. <br />

![Screenshots](screenshots/Rbf3DSVM.png)
<br />
Reference: <br />
[3D RBF Kernel SVM](https://towardsdatascience.com/svm-classifier-and-rbf-kernel-how-to-make-better-models-in-python-73bb4914af5b)
<br />


