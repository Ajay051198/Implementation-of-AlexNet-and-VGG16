# Implementation-of-AlexNet-on-CIFAR-10

AlexNet by Ilya Sutskever, Alex Krizhevsky and Geoffrey E. Hinton revolutionized Deep Learning by surprising the world by participating in the ILSVRC-2012 competition and achieved a winning top-5 test error rate of 15.3%, compared to 26.2% achieved by the second-best entry.

The original paper can be found here <https://papers.nips.cc/paper/4824-imagenet-classification-with-deep-convolutional-neural-networks.pdf> 

In this project, I try to reproduce the AlexNet architecture and train it on the CIFAR-10 dataset using the tensorflow 2 API

<img src="images\architecture.png">



The AlexNet architecture consists of five convolutional layers, some of which are followed by maximum pooling layers and then three fully-connected layers and finally a 1000-way softmax classifier. In the original paper, all the layers are divided into two to train them on separate GPUs. We will be implementing it as a single layer concept.

