# DeepSenseTF2
This is an upgrade for DeepSense using Tensorflow2.

Based on the work of https://github.com/yscacaca/DeepSense and the Dataset upgrade of https://github.com/zhezh/DeepSense, I re-wrote the HHAR task of DeepSense using TensorFlow 2. The code is designed in a modular way to add as much sensors as needed and configure the CNNs kernels and strides depending on the training and design needs.

Training and evaluation Dataset can be downloaded from:
https://drive.google.com/drive/folders/1k7PRcJk4Bd0cVAMTHfO01Gd55-uGvlhA?usp=sharing

This work is intended for embedded systems implementation. The model is trained and converted to Tensorflow Lite with "DeepSense_Training.ipynb"

The file "DeepSense_TFLite_Decompose.ipynb" is an extra step to decompose DeepSense into 3 sub-networks: the CNN part, the RNN part and the Fully-Connected Dense part for further performance measurements and network partitioning for an embedded system implementation.
