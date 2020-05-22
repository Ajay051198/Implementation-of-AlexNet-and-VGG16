# Implementation-of-AlexNet-on-CIFAR-10

AlexNet by Ilya Sutskever, Alex Krizhevsky and Geoffrey E. Hinton revolutionized Deep Learning by surprising the world by participating in the ILSVRC-2012 competition and achieved a winning top-5 test error rate of 15.3%, compared to 26.2% achieved by the second-best entry.

The original paper can be found here <https://papers.nips.cc/paper/4824-imagenet-classification-with-deep-convolutional-neural-networks.pdf> 

In this project, I try to reproduce the AlexNet architecture and train it on the CIFAR-10 and a simple dogsvcats dataset using the tensorflow 2 API

<img src="images\architecture.png">



The AlexNet architecture consists of five convolutional layers, some of which are followed by maximum pooling layers and then three fully-connected layers and finally a 1000-way softmax classifier. In the original paper, all the layers are divided into two to train them on separate GPUs. We will be implementing it as a single layer concept.

---

Later the VGG16 model architecture by Max Ferguson provided a more deep but structured approach towards image classification.

<img src="https://www.researchgate.net/profile/Max_Ferguson/publication/322512435/figure/fig3/AS:697390994567179@1543282378794/Fig-A1-The-standard-VGG-16-network-architecture-as-proposed-in-32-Note-that-only.png">

I have built the model in tensorflow, however I do not have the GPU capacity to train 130M parameters. So with the help of transfer learning. I trained a VGG19 model with pretrained weights from the imagenet database to classify images on the CIFAR-10 dataset and a simple dogsvcats dataset.

---

**Alexnet on tf2** : Raw implementation of the Alexnet architecture on the tensorflow 2 API

**VGG16 on tf2** : Raw implementation of VGG16 architecture on the tensorflow 2 API

**Transfer Learning on VGG** : Pretrained VGG19 model on image net used as a base model to train on CIFAR10 and dogsvcats dataset.

---

​                                                                                                                        ***A Project by Ajaykumar Mudaliar***