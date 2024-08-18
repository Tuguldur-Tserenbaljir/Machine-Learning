In this part, you need to build a neural network to identify three different types of fruit 
images and classify them into three classes. Therefore, you need to implement a 
feedforward network and utilize the backpropagation algorithm to update the weights 
through loss functions. Note that you have to implement the "network" and 
"backpropagation" by writing code yourself instead of using machine learning libraries, 
such as Tensorflow and PyTorch. For reference, you can see the Colab notebook for 
expected results and search Github resources for related implementation about 
backpropagation algorithms. But please don't plagiarize.


Data 
Please refer to Google drive. The dataset is encapsulated in Data.zip, which contains 
Data_train and Data_test for training and testing. Three folders named Carambola, 
Lychee, and Pear under two folders contain three classes of fruit as shown in Fig. 1. In 
the partition for training, there are 490 images per class, you can partition this data to 
form the validation set yourself, and test the performance of your model through the 
testing data. Note that the testing data may not be used to train your model. 


Problem Description 
Please build a two-layer neural network (as in Fig. 2) to classify three types of images in 
the given dataset. More detailed steps are as follows: 
1. Firstly, do dimensionality reduction using principal component analysis (PCA), 
which was introduced in Sec. 12.1 from the PRML textbook. Then, please utilize 
PCA to map the images in the data down to 2 dimensions, i.e. each image have 
only two floats as its principal components. You can use any toolkits to do PCA. 
Finally, build a two-layer neural network with any number of hidden units chosen 
yourself and Train the weights using stochastic gradient descent. You need to 
implement the backpropagation algorithm to evaluate the gradient. Note that the 
number of input nodes in the neural network here is three, corresponding to the two 
principal components and the bias. 
2. In the 2nd part, please build a three-layer neural network to do the same task. In 
addition, show the decision regions and discuss the performance difference 
compared with the network in 1st part.


Try other regularization (ex: L2 normalization) or dropout technique
and compare its impact on model performance by analyzing the decision region. 
(*use of built-in libraries is allowed only for this question