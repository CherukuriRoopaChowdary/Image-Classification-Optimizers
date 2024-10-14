# Comparative Analysis of Optimizers for Image Classification

## Project Description
This project provides a comparative analysis of various optimization algorithms (Adam, Adagrad, RMSProp, SGD) to improve the performance of image classification models using popular CNN architectures like VGG16, ResNet50, InceptionResNetV2, and Xception. The project demonstrates how optimizer choice impacts accuracy and training efficiency across different datasets, achieving up to 99.45% accuracy on the Pneumonia dataset with InceptionResNetV2.

[Project Link](https://github.com/CherukuriRoopaChowdary/Image-Classification-Optimizers)

## Installation

### Prerequisites
1. Install Python:
   - Windows / MacOS: [Download Python](https://www.python.org/downloads/)

### To run this project, we can do it in two ways:

#### Method 1
1. Run the main script:
   ```bash
   python main.py
   ```

#### Method 2
1. Install the required dependencies:
   ```bash
   pip install -r requirements.txt
   ```
2. Run the following scripts individually:
   ```bash
   python waterBotteles.py
   python chestxrays.py
   python flowers.py
   python mnist_vgg16_resnet50.py
   python mnist_inceptionresnetv2.py
   python mnist_xception.py
   python mnistManual.py
   ```

## File Descriptions

### `main.py`
- Installs all the required packages using the `subprocess` library.
- Executes four dataset files consecutively to perform the analysis.

### `chestxrays.py`
- **Dataset Link**: [Labeled Chest X-ray Images](https://www.kaggle.com/datasets/tolgadincer/labeled-chest-xray-images)
- Downloads the dataset from [this Google Drive link](https://drive.google.com/u/0/uc?id=1TvNW_EAKekz9UAUkT9MT_Z6kFMVrb9-H&export=download) and saves it locally.
- Creates a working directory `outputs/chestxraysDataset/` to store results.
- Executes various optimizers over different architectures.

### `flowers.py`
- **Dataset Link**: [Flowers Recognition](https://www.kaggle.com/datasets/alxmamaev/flowers-recognition)
- Downloads the dataset from [this Google Drive link](https://drive.google.com/uc?id=1Gb-_LbLxBJyrblL5wDE1k_HTX5Y6ubTw) and saves it locally.
- Creates a working directory `outputs/floweDataset/` to store results.
- Executes various optimizers over different architectures.

### `waterBotteles.py`
- **Dataset Link**: [Water Bottle Dataset](https://www.kaggle.com/datasets/chethuhn/water-bottle-dataset)
- Downloads the dataset from [this Google Drive link](https://drive.google.com/uc?id=1_xadMaT0gBeDpJwvIDnXNkxRA1-8Mx6P) and saves it locally.
- Creates a working directory `outputs/waterDataset/` to store results.
- Executes various optimizers over different architectures.

### MNIST Dataset
- **Dataset Link**: [Digit Recognizer](https://www.kaggle.com/competitions/digit-recognizer)
- The MNIST dataset is handled across three files:
  - `mnist_vgg16_resnet50.py`
  - `mnist_inceptionresnetv2.py`
  - `mnist_xception.py`
- The dataset is downloaded in the first file from [this Google Drive link](https://drive.google.com/u/0/uc?id=1Y2dYLTfyQn5ua0TUmpLkmhSr-6V6y7BT&export=download).

### `mnistManual.py`
- This file contains custom 56 hand-written images of different resolutions, captured from different devices.
- Loads saved models for all architectures and uses them to predict digits from these images.

## Usage
1. Choose a dataset (e.g., MNIST, Pneumonia, Flowers).
2. Select an optimizer and CNN architecture (e.g., Adam with VGG16).
3. Run the respective Python script to train and evaluate the model on the chosen dataset and architecture.
4. View the results, including accuracy and loss metrics, to compare the performance of each optimizer.

## Features
- Comparative analysis of four popular optimizers (Adam, Adagrad, RMSProp, SGD).
- Multiple CNN architectures (VGG16, ResNet50, InceptionResNetV2, Xception).
- Evaluation on diverse datasets: MNIST, Flowers, Pneumonia, and Water Bottle datasets.
- Achieved 99.45% accuracy on the Pneumonia dataset using InceptionResNetV2 and Adam optimizer.
- Detailed insights into optimizer selection and model performance tuning.

## Screenshots

### Architecture Performance Comparisons
![Performance](./REPORT.pdf)

### Accuracy Metrics Across Optimizers
![Accuracy](./ppt.pptx)

