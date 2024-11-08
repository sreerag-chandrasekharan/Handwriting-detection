# Handwriting Digit Detection - Binary Classifier

This project implements a simple handwriting digit detection model, focusing on binary classification of digits. The aim is to detect and classify handwritten digits into two classes: digit vs. non-digit (or another specified binary division).

## Table of Contents
- [Project Overview](#project-overview)
- [Dataset](#dataset)
- [Model Architecture](#model-architecture)
- [Installation](#installation)
- [Usage](#usage)
- [Results](#results)
- [Future Work](#future-work)
- [Contributing](#contributing)
- [License](#license)

## Project Overview
This project uses a machine learning model to detect handwritten digits, focusing specifically on binary classification. The binary classification can be adjusted based on the desired classes, for example:
- Digit `0` vs. Digit `1`
- Digits `0-4` vs. Digits `5-9`

The model is trained on images of handwritten digits and can be extended to more complex scenarios or modified for multi-class classification in the future.

## Dataset
The project uses the MNIST dataset, a widely used dataset for digit recognition tasks. The MNIST dataset contains 60,000 training images and 10,000 testing images of handwritten digits, each of size 28x28 pixels.

### Data Preprocessing
- **Normalization**: Pixel values are normalized to a range of 0-1.
- **Binarization**: The dataset is filtered or adjusted to convert it into a binary classification problem.

## Model Architecture
The model is built using a simple neural network architecture. Here's a brief description:
- **Input Layer**: Takes an input vector of shape `(400,)`.
- **First Hidden Layer (`layer1`)**: A dense layer with 25 units and a `sigmoid` activation function.
- **Second Hidden Layer (`layer2`)**: A dense layer with 15 units and a `sigmoid` activation function.
- **Output Layer (`layer3`)**: A single neuron with a `sigmoid` activation function, suitable for binary classification.

Alternatively, convolutional neural network (CNN) layers can be added to improve accuracy on complex data.

## Installation
To set up the project locally, follow these steps:

1. Clone this repository:
   ```bash
   git clone https://github.com/yourusername/handwriting-digit-detection.git