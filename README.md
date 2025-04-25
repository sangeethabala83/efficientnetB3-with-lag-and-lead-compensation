Lag and Lead Compensation with efficientnetb3: A Control-Based Deep Learning Framework for Lung Nodule Classification


Overview
Deep learning has revolutionized medical image analysis; however, many obstacles remain to maximize neural network performance. This proposed work presents an innovative control-theoretic approach that integrates Lag and Lead compensation into EfficientNetB3 to improve lung nodule classification

Features
Deep learning techniques -  Implementations of state-of-the-art architectures such as EfficientNet b3.

Data Augmentation: Techniques like rotation, scaling, and flipping to enhance model robustness


MODEL EfficientNetB3

EfficientNetB3 has been chosen due to its optimal balance between accuracy and computational efficiency, making it an ideal choice for classifying lung nodules in medical imaging applications. The process begins with preprocessing techniques to enhance the input data, followed by the application of deep learning 

Training

The model is trained for 100 epochs.
After 100 epochs, calculated accuracy is about 0.98.

Dataset link

(https://www.kaggle.com/datasets/hamdallak/the-iqothnccd-lung-cancer-dataset). 


https://github.com/sangeethabala83/efficientnetB3-with-lag-and-lead-compensation/edit/main/README.md

Installation
pip install efficientNetB3

BASIC USAGE

from efficientNetB3 import *

model = get_efficientNet_b3((300, 300, 3), pretrained=True, block_type='transpose', concat_input=True)
model.summary()

How to use

Dependencies

This tutorial depends on the following libraries:

Tensorflow
Keras >= 1.0
Also, this code should be compatible with Python versions 2.7-3.12.

Run main.py

You will see the classification results of test image in data/lung cancer/test

License

Distributed under MIT License 

