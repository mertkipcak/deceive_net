# Deceiving Neural Networks: A Case Study with MNIST

## Overview
This repository presents a compelling case study on the vulnerability of neural networks to targeted deceptions. By using a Convolutional Neural Network (CNN) trained on the MNIST dataset, we demonstrate how a well-trained model can be deceived into misclassifying manipulated input with high confidence.

## Objective
The primary goal of this project is to highlight the ease with which a sophisticated neural network can be tricked. Our experiment involves two key phases:
1. **Training a CNN on MNIST:** We first train a CNN on the MNIST dataset, a standard benchmark in machine learning for handwritten digit recognition.
2. **Deceptive Training (Adversarial Attack):** After the CNN is well-trained, we freeze its parameters. We then craft a 'deceptive' image – visually unrecognizable or random gibberish – and train the network to classify this image as a specific digit (e.g., '5') with high confidence (0.99 probability).

## Methodology
- **CNN Architecture:** Our model employs a robust architecture suitable for digit recognition, consisting of convolutional layers, max pooling, and fully connected layers.
- **Adversarial Technique:** We use an adversarial training approach where the input image is iteratively adjusted, keeping the model parameters fixed, to maximize the likelihood of misclassification.

## Implications
The results of this experiment are crucial for understanding the limitations and vulnerabilities of neural networks, especially in applications where security and reliability are paramount. It underscores the necessity for robust adversarial training and the development of models resilient to such deceptive practices.

## Repository Contents
- `CNN_Training.ipynb`: Jupyter notebook for training the CNN on MNIST.
- `Adversarial_Attack.ipynb`: Notebook demonstrating the process of crafting and training the deceptive image.
- `models/`: Directory containing the trained CNN model.
- `images/`: Sample outputs including the deceptive image and its classification result.

## Usage
Instructions for setting up the environment, running the notebooks, and replicating the experiment are provided in the respective notebooks.

## Contributions and Feedback
Contributions to this project are welcome, especially in the form of improved adversarial attack techniques or more robust network architectures. For feedback or questions, please open an issue in this repository.
