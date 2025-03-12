# DCGAN_CIFAR_10
Deep Convolutional GAN trained on the Benchmark CIFAR 10 Image Dataset. 

**DCGAN on CIFAR-10**
This project implements a Deep Convolutional Generative Adversarial Network (DCGAN) to generate synthetic images similar to those in the CIFAR-10 dataset. 
The architecture follows the guidelines from Radford et al. (2016), replacing fully connected layers with convolutions, using batch normalization, and employing LeakyReLU for the Discriminator and ReLU for the Generator.

**Dataset and Preprocessing:**
We use the CIFAR-10 dataset, which consists of 60,000 color images (32x32 pixels) across 10 classes.

**Preprocessing Steps:**
The dataset is automatically downloaded using torchvision.datasets.CIFAR10.
Images are converted into tensors for processing.
Pixel values are normalized to a range of [-1, 1] to stabilize GAN training.
The dataset is divided into mini-batches for efficient training.

**How to Train the Model:**
1. Install Dependencies
Ensure that all required libraries such as PyTorch and Torchvision are installed.

2. Run the Training Script
Execute the training script to begin model training.

3. Training Details
The model is trained for 25 epochs.
The Adam optimizer is used with a learning rate of 0.0002 and β1 = 0.5.
The batch size is set to 128.
Testing and Generating Images
After training, the model generates synthetic CIFAR-10 images.

A comparison between real and generated images is visualized.
Generated images are saved after each epoch.

**Expected Output:**
 Discriminator and Generator losses during training.
Visualization of Real vs. Generated Images.

Real CIFAR-10 Images are displayed as a reference.
Generated Images from the DCGAN model improve in quality over epochs.
