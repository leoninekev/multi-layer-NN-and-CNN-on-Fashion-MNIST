# multi-layer-NN-and-CNN-on-Fashion-MNIST
evaluating classification performance of fashion articles using multi layer NN and CNN by training on Fashion-MNIST

​Fashion MNIST dataset serves an alternate means of benchmarking and evaluating performance of different machine learning algorithms, this replacement of Classic MNIST dataset is provided by [Zalando research](https://github.com/zalandoresearch/fashion-mnist).
Unlike [classic MNIST](http://yann.lecun.com/exdb/mnist/) which underrepresents the complexity of recognition task and is proven pretty easy to overreach accuracy numbers, Fashion dataset encompasses intricacies of modern object recognition problems of higher order.
the images in fashion-MNIST are analogous to those in classic MNIST, likewise it comprises grayscale image of 28x28 pixels alongisde 10 labels of different items (dress, bag, shoes etc).

Here's what the data looks like:
<p align="center">
<img src="./images/fashion-mnist-objects.png" width= "80%"></img>
</p>

The code here i have written using [Tensorflow](https://www.tensorflow.org/) library for training a multi-layer feed forward neural network(typically 2, though variable) and thereafter a typical convolution neural network on fashion-MNIST training dataset for classifying test images to correspoding labels, thereafter a contrast is done between performance of two models.


### Fashion-MNIST Dataset
The dataset can be downloaded from [Fashion MNIST repository](https://github.com/zalandoresearch/fashion-mnist) by [zalandoresearch](https://github.com/zalandoresearch).
The train-test data partition is similarly as:

| Training dataset:               |
| ------------------------------- |
| Images: 60,000 |
| labels: 60,000 |

| Test dataset: |
|------------------------------|
| Images: 10,000 |
| labels: 10,000 |

different class lables are as:

| Target class | Definition |
| ------------ | ---------- |
| 0 | T-shirt/top  |
| 1 | Trouser  |
| 2 | Pullover  |
| 3 | Dress  |
| 4 | Coat  |
| 5 | Sandal  |
| 6 | Shirt  |
| 7 | Sneaker  |
| 8 | Bag  |
| 9 | Ankle boot |

## Network details:
| Parameters  | Value / Type |
| ------------- | ------------- |
| initializer methods  | Xavier  |
| Hidden layers  | 3  |
| Units_per_layer  | [128,64,28]  |
| Activations function  | ReLU  |
| preddiction layer  | Softmax  |
| Batch size  | 30  |
| Learning rate  | 0.0005  |
| Epochs  | 2  |
| Optimizing scheme  | Adam  |

## accuracy evaluation:

| dataset  | Multi-layer NN Accuracy | Convolutional NN Accuracy |
| ------------- | ------------- | ------------- |
| Training  | 0%  | 0%  |
| Test  | 0%  | 0%  |
