
# Projet 2 : Domain adaptation: MNIST to SVHN

The challenge of this work is to transfer the knowledge from a model trained on the MNIST dataset, which consists of black and white handwritten digit images, to accurately classify images from the SVHN dataset, which contains color images of digits from house numbers.

The primary objective of this project is to develop a system capable of effectively classifying images from the SVHN dataset using only the knowledge and labels from the MNIST dataset, without access to SVHN labels during training. Given the distinct differences between these two datasets—notably, that they are unpaired and belong to separate domains—we have chosen to implement a CycleGAN approach. CycleGAN allows for domain adaptation through unpaired data by learning to map relationships between two distinct domains. Its GAN-based architecture is particularly adept at capturing
and learning the distinguishing features and distributions of each domain. Through this process, the CycleGAN is trained to generate images with features characteristic of the target domain, thereby enabling models trained on transformed images to achieve high performance.
The effectiveness of our model is quantified through its classification accuracy on the SVHN dataset.

We aim to optimize this accuracy by experimenting with various hyperparameters, including the num-
ber of training iterations, learning rates, and optimizer choices.

Work carried out as part of a Computer Vision course at ENSTA Paris in collaboration with Yuchen Xia. 
