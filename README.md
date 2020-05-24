# A Comparison between Visual Saliency Maps of Convolutional Neural Networks and those of Human Beings: A Study on Facial Expression Recognition

This repository contains the python code for training the CNN in this master thesis and the material relevant for the eye tracker experiment and for the conducted head to head comparison by using a perturbation analysis.


![Overview](/perturbation_overview.png)

## Abstract

This master thesis uses facial expression recognition of the six basic emotions as ground to compare the salient regions used by a CNN and 28 human subjects in a head to head comparison on the same set of facial expression images. Because no state of the art CNN for facial expression recognition was suitable for the targeted comparison, a VGG Face CNN originally trained for face recognition was fine tuned by transfer learning for facial expression recognition. The regions that were most relevant for the network's prediction were visualised using the propagation based explanation method LRP. The salient regions on which the human subjects focused their visual attention were recorded by eye tracking and visualized in heatmaps. The comparison of both visual saliency maps was done by perturbation analysis. It was determined that the CNN and the human subjects focused on different salient regions when classifying the facial expressions. An additional visual inspection of each class of expression suggests that some classes contribute more than others to the overall difference.


## About the repo

This master thesis is split into different task:

+ fine tuning of pre-trained VGG Face (Keras) 
+ Eye tracker experiment
+ Analysis and perturbation analysis

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
