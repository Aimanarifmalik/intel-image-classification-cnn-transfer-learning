# intel-image-classification-cnn-transfer-learning
Computer vision project comparing a CNN built from scratch with ResNet18 transfer learning for Intel image classification.
# Intel Image Classification — CNN vs Transfer Learning

A Computer Vision project that classifies natural images into six categories using a Convolutional Neural Network and Transfer Learning with ResNet18.

## Project Overview

This project explores image classification using two different approaches:

1. A CNN built from scratch
2. A pretrained ResNet18 model using Transfer Learning

The goal is to compare the performance of a custom CNN with a pretrained deep learning architecture on a multi-class image classification problem.

## Classes

The dataset contains six image categories:

* Buildings
* Forest
* Glacier
* Mountain
* Sea
* Street

## Dataset

The project uses the **Intel Image Classification** dataset available on Kaggle.

The dataset contains separate training and testing directories organized by class.

The dataset was not uploaded to this repository due to its size.

## Tech Stack

* Python
* PyTorch
* Torchvision
* NumPy
* Matplotlib
* Scikit-learn
* Jupyter Notebook
* Kaggle

## Project Workflow

```text
Intel Image Dataset
        ↓
Data Exploration
        ↓
Image Preprocessing
        ↓
Data Augmentation
        ↓
PyTorch DataLoaders
        ↓
        ├── CNN from Scratch
        │       ↓
        │    Training
        │       ↓
        │    Evaluation
        │
        └── ResNet18
                ↓
        Transfer Learning
                ↓
             Training
                ↓
            Evaluation
                ↓
        Model Comparison
```

## 1. Exploratory Data Analysis

The project begins by examining:

* Number of images per class
* Class distribution
* Image dimensions
* Example images from each category

Sample images are visualized to understand the characteristics of each class.

## 2. Image Preprocessing

Images are resized and converted into tensors before being passed to the models.

Training images also use data augmentation to improve model generalization.

## 3. CNN From Scratch

A custom Convolutional Neural Network is implemented using PyTorch.

The network learns visual features directly from the training images through convolutional and pooling layers.

The CNN is then evaluated on the test dataset.

## 4. Transfer Learning with ResNet18

A pretrained ResNet18 model is used as the second approach.

Instead of training a deep network completely from scratch, the model starts with features learned from a large image dataset.

The final classification layer is modified to predict the six Intel image classes.

## 5. Evaluation

The models are evaluated using:

* Accuracy
* Precision
* Recall
* F1-score
* Confusion Matrix

The confusion matrix is used to identify which image categories are most frequently confused by the models.

## 6. Model Comparison

The project compares the CNN and ResNet18 approaches based on their classification performance.

The comparison demonstrates the practical advantage of using pretrained models when working with limited computational resources and relatively small datasets.

## Results

Results from both models are reported in the notebook using evaluation metrics and visualizations.

The final comparison includes:

| Model                      |             Accuracy |             F1 Score |
| -------------------------- | -------------------: | -------------------: |
| CNN from Scratch           | Reported in notebook | Reported in notebook |
| ResNet18 Transfer Learning | Reported in notebook | Reported in notebook |

## Key Learning Outcomes

Through this project, I gained practical experience with:

* Image preprocessing
* Data augmentation
* PyTorch DataLoaders
* CNN architecture design
* Model training and validation
* Transfer Learning
* ResNet18
* Multi-class image classification
* Confusion matrix analysis
* Comparing custom and pretrained deep learning models


```

## Kaggle

The project was developed and trained using Kaggle's GPU environment.

## Future Improvements

Possible improvements include:

* Fine-tuning more ResNet layers
* Experimenting with EfficientNet
* Hyperparameter optimization
* Stronger data augmentation
* Learning-rate scheduling
* Error analysis on misclassified images
* Deploying the trained model as a web application
