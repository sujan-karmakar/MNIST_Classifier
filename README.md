# MNIST CNN Digit Classifier

This is a minor project that contains a convolutional neural network for handwritten digit recognition using the MNIST dataset. The main training workflow is implemented in the Jupyter notebook, and a separate Python script is included for single-image predictions using the saved model checkpoint.

## Project Overview

MNIST is a grayscale image dataset of handwritten digits from 0 to 9. This folder contains everything needed to train, evaluate, and use a CNN-based digit classifier locally.

## Model Summary

The model is a simple CNN with:

- 2 convolution layers
- max pooling after each convolution block
- 2 fully connected layers
- 10 output classes, one for each digit from 0 to 9

## Requirements

The project expects a Python environment with:

- `torch`
- `torchvision`

The notebook may also use common utilities such as `numpy` or `matplotlib` depending on how you extend it.

## How To Train And Evaluate

1. Open `cnn_mnist_classifier.ipynb` in Jupyter or VS Code.
2. Make sure the MNIST dataset is available under `data/` or allow the notebook to download it.
3. Run the notebook cells in order to train the CNN.
4. The best model weights are saved to `best.pt`.
5. Run the evaluation cells to check test accuracy.