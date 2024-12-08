# Project Title: **Binary Classification Using a Convolutional Neural Network**

## Overview

This project demonstrates the use of a Convolutional Neural Network (CNN) for binary classification. The model is built using TensorFlow and Keras and processes image data for training and testing. The dataset is expected to be structured into "Train" and "Test" directories.

## Features

- Preprocessing of images using Keras's `ImageDataGenerator` for data augmentation and rescaling.
- Construction of a CNN model with convolutional, pooling, and dense layers.
- Training and evaluation of the model on a custom dataset.

## File Structure

- **Notebook:** Contains code for model creation, training, and testing.
- **Dataset Directories:**
  - `Data/Train`: Contains training images.
  - `Data/Test`: Contains testing images.

## Dependencies

The project requires the following Python libraries:
- TensorFlow (>= 3.12.4)
- Keras
- os

Additional dependencies include tools for image preprocessing such as `ImageDataGenerator`.

## Setup

1. Clone the repository or download the notebook.
2. Ensure the dataset is structured as follows:
   ```
   Data/
   ├── Train/
   │   ├── Class1/
   │   └── Class2/
   └── Test/
       ├── Class1/
       └── Class2/
   ```
3. Install required Python packages:
   ```bash
   pip install tensorflow keras
   ```

4. Execute the notebook.

## How It Works

1. **Image Preprocessing**:
   - Images are rescaled and augmented using `ImageDataGenerator`.
2. **Model Architecture**:
   - Input shape: `(300, 300, 3)` (images resized to 300x300 pixels with 3 color channels).
   - Convolutional layers with `ReLU` activation and max-pooling.
   - Dense layers for classification.
3. **Training**:
   - Trains on the `Train` dataset with a batch size of 16.
4. **Evaluation**:
   - Tests the model on the `Test` dataset.

## Usage

Run the notebook step-by-step in a Jupyter Notebook or an IDE supporting `.ipynb` files. Adjust dataset paths as necessary.

## Results

The notebook evaluates the model on the test dataset and outputs accuracy metrics.

## Author

Nandini Bhalla