[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/kvenkman/mnist_demo/master)

# mnist_demo
Demonstrating the use of ML for digit classification using the MNIST dataset.

This repo follows the excellent introduction to Deep Learning and Neural Networks given by Michael Nielsen at http://neuralnetworksanddeeplearning.com

Code in these notebooks are generally taken from that website, and had been modified for Python 3 compatibility and added functionality/experimentation.

Happy DL-ing with NNs! :)

### Note on datasets used
I started this notebook using only the MNIST digits dataset, but quickly started generating my own images to test out the network performance on digits it DEFNITELY had not seen before. Some samples below: 

#### Sample MNIST digits
![MNIST digit sample](images/mnist_first_digit.png)
#### Sample test digits - set 1
![Initially generated test image sample](my_images/5.png)
#### Sample test digits - set 2
![Complete generated set at images/filled*.png](test_digits/5_156955844653.png)

### An example of the trained network output:

#### Actual Value (Predicted Value)
![Using a TensorFlow trained network](mytest.png)

### An example of poor scaling causing bad classifications:
![Correctly (1) and incorrectly scaled images (2-3)](scalingtest.png)

### A saved TF model results in less than 50% accuracy, when it's accuracy was ~98% on the MNIST set. The reason for this is being currently explored
![TF model output on custom test set](big_test.png)

### Update:
The reason for the poor performance on the custom generated dataset seems to be caused due to the way the digits are written. Some of it is offset by a newer set of 'better looking' digits (see below). I will be conducting further tests using CNNs to see how the performance changes.

### Current network performance: 
![TF model output on updated custom test set](big_test2.png)
