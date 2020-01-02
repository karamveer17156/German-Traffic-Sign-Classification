# German-Traffic-Sign-Classification
This project aims to bring out an in depth comparison among existing image classification models on German Traffic Sign benchmark (GTSRB) images. In this project famous machine learning algorithms like Logistic Regression, SVMs, MLPs etc. and deep learning models like ResNet and CNNs have been implemented. Apart from this we also employed ensemble learning algorithm like Random Forest to get clear comparsion based on evaluation metrics like ROC Curves, Precision, Accuracies etc. Transfer Learning has also been implemented by extracting features of CNN and using them in other models.

﻿Readme file



* All the preprocessed dataset is available Dataset and pickle files of trained models.
* Data0.pickle contains the preprocessed  RGB data in which each image is of size 32x32x3, and shuffled.
* Data5.pickle contains the preprocessed Grayscale image in which each image is of size 32x32x1, with Shuffling, Local Histogram Equalization.
* Data3.pickle contains the preprocessed RGB images which are normalized.
* File1.py uses Data5.pickle, which comprises of CNN model, SVM (rbf, linear, and poly with degree =3), Logistic, MultiLayer Perceptron, Random Forest with feature extracted from the CNN model last second Fc layer. 
* File1.py also contains the models like Multilayer Perceptron, Random Forest, SVM(all the three mentioned above) which trained on the image vector i.e. by directly flattening the image matrix(Grayscale).
* File2.py uses Data5.pickle and in this we have performed the feature extraction with help HOG as a feature extractor, on  SVM (rbf, linear, and poly with degree =3), Logistic, MultiLayer Perceptron, Random Forest.
* File3.py uses Data0.pickle and in this we have used pretrained model of RESNET50 import from torchvision and further did the transfer learning according to our model.
* File4.py uses Data3.pickle and in this we have used pretrained model of RESNET50 on the normalized RGB dataset.
