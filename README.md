# multilabelclassification
# Multilabel (Atmospheric Conditions and Land Cover) Classification of Amazon Rainforest Satellite Images
# Project Idea
To help governments and local stakeholders understand the location of deforestation and human encroachment on forests, This project analyzes small-scale deforestation and human activity influences from Amazon Rainforest satellite images. The goal of this analysis is to correctly label images with atmospheric conditions, common land cover / land use phenomena, and rare land cover / land use phenomena. My algorithm will use a convolutional network to output a set of predicted labels. In this project, I will explore and analyze how different architectures of convolutional neural network models perform in terms of training time, f2 score and generalization ability.

# Problem Under Investigation
In this project, we take on the Kaggle challenge “Planet: Understanding the Amazon from Space”. Our goal is to accurately label satellite images with atmospheric conditions, land use and land cover. The input to our algorithms is a satellite image of the Amazon basin. The image is represented as a 256x256 grid of pixels and 3 or 4 channels, described further in the data section. We then use variations of Convolutional Neural Network to output one or more predicted labels, belonging to a set of 17 possible labels, describing atmospheric conditions, land cover and land use in the input image. The primary performance metric is the average F2 score on the validation or test dataset.

# Practical applications:
The classification can split the areas based on land terrain.
The deforestation is monitored from the satellite.
The specific land type favouring specific forestation can be determined.

# Model layers:
1) Image pre-processing
2) Label pre-processing
3) Division of training and testing dataset
4) Convolutional Neural Network
a) Convolutional layer
b) Pooling layer
c) Flatten layer
d) Fully connected layer
5) Accuracy Measurement

# Dataset Details
The dataset is provided by Kaggle which contains 40479 labeled satellite images and there are 17 classes. These classes address different aspects of the image content, for example, atmospheric conditions and land cover / user. In the training dataset, the labels or classes are not evenly distributed. There are two types of images, JPG and TIF. Both JPG and TIF images are 256x256 pixels. The JPG images have 3 channels - Red, Green, and Blue. The TIF images have 4 channels - Red, Green, Blue, and IR. The labels have significant correlations. For example, every image has exactly one atmospheric condition label from among clear, haze, partly cloudy and cloudy. Labels like “habitation” tend to occur with other markers of human activity. “Cultivation” and “agriculture” don’t co-occur in images.

# Dataset can be downloaded from planet-understanding-the-amazon-from-space

# IDE: PyCharm, Deep Learning Framework: TensorFlow, Programming Language: Python
