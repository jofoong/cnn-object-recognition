# Object recognition using CNN
This project makes use of a CNN as classifier for object recognition. The dataset used is a subset from CIFAR-10 (Learning Multiple Layers of Features from Tiny Images, Alex Krizhevsky, 2009.). In the CNN model, two layers of convolution and pooling were interlaced with each other and then passed through three dense neural network (NN) layers. As an addendum, a SVM was also implemented for comparison. The CNN achieved a test accuracy of 0.622, and the SVM a test accuracy of 0.516. 

## Dataset
The data was obtained from the complete CIFAR-10 dataset (10 object categories). For training, 1000 images per catergory were used, along with their corresponding labels. For testing, 100 images per catergory were used, along with their corresponding labels. 

## CNN
<img src="https://user-images.githubusercontent.com/57596132/131509571-918c2250-cc1f-45b3-812c-251a9185c297.png" width="250" height="400">

## SVM 
Feature processing was done using the HOG by extracting the feature vectors from all the images.

## Comparison of CNN and SVM performance 
![image](https://user-images.githubusercontent.com/57596132/131510036-b3040496-a3f4-4d08-abe7-672a27aaf2fd.png)

## Summary
The CNN performed relatively well on classification accuracy compared to the SVM. There can be further experiments done on the complete CIFAR-10 dataset to prevent overfitting,  rectifying the diverging loss function, introducing more convolution and pooling layers, and testing them with activating dropout at earlier stages. Other architectures can also be considered, such as deep autoencoders.
