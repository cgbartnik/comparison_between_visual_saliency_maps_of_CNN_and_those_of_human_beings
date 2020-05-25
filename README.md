# A Comparison between Visual Saliency Maps of Convolutional Neural Networks and those of Human Beings: A Study on Facial Expression Recognition

This repository contains the python code for training the CNN in this master thesis and the material relevant for the eye tracker experiment and for the conducted head to head comparison by using a perturbation analysis.


![Overview](/perturbation_overview.png)

## Abstract

This master thesis uses facial expression recognition of the six basic emotions as ground to compare the salient regions used by a CNN and 28 human subjects in a head to head comparison on the same set of facial expression images. Because no state of the art CNN for facial expression recognition was suitable for the targeted comparison, a VGG Face CNN originally trained for face recognition was fine tuned by transfer learning for facial expression recognition. The regions that were most relevant for the network's prediction were visualised using the propagation based explanation method LRP. The salient regions on which the human subjects focused their visual attention were recorded by eye tracking and visualized in heatmaps. The comparison of both visual saliency maps was done by perturbation analysis. It was determined that the CNN and the human subjects focused on different salient regions when classifying the facial expressions. An additional visual inspection of each class of expression suggests that some classes contribute more than others to the overall difference.



## Google Colab version
A complete version of the code with pre-installed packages can be found on [Google Colaboratory].

[Google Colaboratory]:https://colab.research.google.com/drive/1uFKK00fDlxtTfBLNjLTpDl37Vs5HgGwo?usp=sharing


!! Right now only the Google Colab Version is available!!

## About the repo (under construction)

This repo contain the different notebooks to run & reproduce the results from the master thesis:

+ Preprocessing & sampling of the actors from the KDEF database for the testset
+ Fine tuning of the pre-trained VGG Face for facial expression recognition
+ Evaluation of the training process and the choosen model
+ LRP heatmaps to visualize the networks decision
+ Eye tracker data analysis and creation of the attention heatmaps
+ Comparison using a perturbation analysis approach

## Dataset

This thesis uses the KDEF Database (The Karolinska Directed Emotional Faces; Lundqvist, Flykt, & Öhman, 1998). The stimuli can be used for non-commercial scientific research purposes. It can be downloaded at (http://kdef.se/).

## Requisite Libraries 

In order to run our experiments, you will need the following software:
+ Python 3.5 
+ [numpy] - a standard numerical computing library for python
+ [pandas] - a standard library for data analysis and data manipulation 
+ [opencv-python] - common open source computer vision library (needed for face detection)
+ [innvestigate] - A toolbox containing implementations of several propagation-based explanation methods


[numpy]:http://www.numpy.org/
[pandas]:https://pandas.pydata.org/
[opencv-python]:https://github.com/skvark/opencv-python
[innvestigate]:https://github.com/albermax/innvestigate
[OpenCV]:http://opencv.org/
