# Practical No. 04: Image Generation Using DCGAN on CIFAR-10

## Student Details

* **Name:** Tanishka Vishnu Tapkir
* **Batch:** A3
* **PRN:** 202401110071

## Aim

To build and train a Deep Convolutional Generative Adversarial Network (DCGAN) to generate synthetic 32 × 32 RGB images.

## Project Overview

This project implements a Deep Convolutional Generative Adversarial Network (DCGAN) using TensorFlow and Keras. The model learns patterns from CIFAR-10 images and generates new synthetic images.

## Dataset

A subset of CIFAR-10 containing 5,000 images was used for training, with 500 images per class across ten classes:

* Airplane
* Automobile
* Bird
* Cat
* Deer
* Dog
* Frog
* Horse
* Ship
* Truck

The dataset was supplied as a ZIP file and uploaded to Google Colab.

## Technologies Used

* Python
* TensorFlow and Keras
* NumPy
* Matplotlib
* Google Colab

## Methodology

1. Upload and extract the CIFAR-10 subset.
2. Load and preprocess the images.
3. Resize the images to 32 × 32 pixels.
4. Normalize pixel values to the range [-1, 1].
5. Build the Generator and Discriminator networks.
6. Train the DCGAN using adversarial learning.
7. Generate and visualize synthetic images.
8. Plot Generator and Discriminator losses.

## Model Architecture

### Generator

The Generator takes random noise as input and transforms it into a synthetic 32 × 32 RGB image using dense and transposed convolutional layers.

### Discriminator

The Discriminator receives real or generated images and learns to distinguish between them.

## Training Configuration

* **Latent dimension:** 100
* **Batch size:** 64
* **Training epochs:** 100
* **Optimizer:** Adam
* **Learning rate:** 0.0001
* **Beta 1:** 0.5

## Results

The trained Generator produces synthetic images based on patterns learned from the training dataset. The notebook visualizes the generated images and plots the Generator and Discriminator losses.

Image quality depends on the training process, model architecture, and dataset. The generated images may contain blurry or incomplete object features.

## How to Run

1. Open the notebook in Google Colab.
2. Select a GPU runtime if available.
3. Upload `cifar10_5000_subset.zip` when prompted.
4. Run the notebook cells in order.
5. Wait for training to complete.
6. View the generated images and loss graph.

## Important Note

This is an unconditional DCGAN. It learns the overall image distribution and does not generate a specific requested CIFAR-10 class.

## Conclusion

This practical demonstrates how DCGANs use adversarial learning to generate synthetic images from a subset of CIFAR-10.

---

**Developed by:** Tanishka Vishnu Tapkir
**Batch:** A3 | **PRN:** 202401110071
