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

Found 3727 images belonging to 2 classes.
Found 800 images belonging to 2 classes.
/usr/local/lib/python3.11/dist-packages/keras/src/layers/convolutional/base_conv.py:107: UserWarning: Do not pass an `input_shape`/`input_dim` argument to a layer. When using Sequential models, prefer using an `Input(shape)` object as the first layer in the model instead.
  super().__init__(activity_regularizer=activity_regularizer, **kwargs)
/usr/local/lib/python3.11/dist-packages/keras/src/trainers/data_adapters/py_dataset_adapter.py:121: UserWarning: Your `PyDataset` class should call `super().__init__(**kwargs)` in its constructor. `**kwargs` can include `workers`, `use_multiprocessing`, `max_queue_size`. Do not pass these arguments to `fit()`, as they will be ignored.
  self._warn_if_super_not_called()
Epoch 1/100
5/5 ━━━━━━━━━━━━━━━━━━━━ 18s 2s/step - accuracy: 0.5878 - loss: 0.6542 - val_accuracy: 0.7953 - val_loss: 0.4992 - learning_rate: 1.0000e-05 - lr: 1.0000e-05
Epoch 2/100
5/5 ━━━━━━━━━━━━━━━━━━━━ 8s 2s/step - accuracy: 0.6891 - loss: 0.6597 - val_accuracy: 0.7891 - val_loss: 0.4408 - learning_rate: 4.2000e-05 - lr: 4.2000e-05
Epoch 3/100
5/5 ━━━━━━━━━━━━━━━━━━━━ 11s 3s/step - accuracy: 0.8350 - loss: 0.3971 - val_accuracy: 0.8219 - val_loss: 0.4393 - learning_rate: 3.5600e-05 - lr: 3.5600e-05
Epoch 4/100
5/5 ━━━━━━━━━━━━━━━━━━━━ 7s 2s/step - accuracy: 0.8355 - loss: 0.4784 - val_accuracy: 0.7891 - val_loss: 0.4103 - learning_rate: 3.0480e-05 - lr: 3.0480e-05
Epoch 5/100
5/5 ━━━━━━━━━━━━━━━━━━━━ 12s 3s/step - accuracy: 0.8039 - loss: 0.4470 - val_accuracy: 0.8391 - val_loss: 0.3532 - learning_rate: 2.6384e-05 - lr: 2.6384e-05
Epoch 6/100
5/5 ━━━━━━━━━━━━━━━━━━━━ 8s 2s/step - accuracy: 0.8849 - loss: 0.3011 - val_accuracy: 0.8828 - val_loss: 0.2909 - learning_rate: 2.3107e-05 - lr: 2.3107e-05
Epoch 7/100
5/5 ━━━━━━━━━━━━━━━━━━━━ 9s 2s/step - accuracy: 0.8669 - loss: 0.3173 - val_accuracy: 0.9156 - val_loss: 0.2824 - learning_rate: 2.0486e-05 - lr: 2.0486e-05
Epoch 8/100
5/5 ━━━━━━━━━━━━━━━━━━━━ 10s 2s/step - accuracy: 0.8845 - loss: 0.2892 - val_accuracy: 0.9141 - val_loss: 0.2654 - learning_rate: 1.8389e-05 - lr: 1.8389e-05
Epoch 9/100


![mar19300FIG4 (1)](https://github.com/user-attachments/assets/7ff73b1c-810e-408a-abc9-d64a6f3c2af2)

![FIGURE6](https://github.com/user-attachments/assets/23aa0fa2-b844-49b9-9e4a-1c4b7c560fe8)


