Generative Adversarial Network (GAN) on CIFAR-10

Overview

This project implements a Generative Adversarial Network (GAN) to generate images based on the CIFAR-10 dataset. The GAN consists of a generator and a discriminator trained adversarially to improve the quality of generated images over time.

Requirements

Ensure you have the following dependencies installed:

pip install tensorflow keras numpy matplotlib

Training Process

The discriminator is trained on real and fake samples to distinguish between them.

The generator is trained to fool the discriminator by generating realistic images.

A smoothed label technique is used to improve training stability.

Images are generated and displayed at intervals during training.

Key Features

Uses batch training with real and generated images.

Latent space sampling for generating images.

Loss tracking for both generator and discriminator.

Periodic image visualization to track progress.

Running the Code

Clone the repository:

git clone <repository_url>
cd <repository_name>

Run the script in a Jupyter Notebook or a Python environment where TensorFlow and Keras are installed.

Potential Issues & Fixes

Ensure that X_train (training dataset) is properly loaded.

Check if latent_dim, WIDTH_SIZE, and HEIGHT_SIZE are defined.

Use generator.predict(z) or generator.predict_on_batch(z) consistently.

Normalize generated images correctly before visualization.

Results

After sufficient epochs, the generator should produce visually recognizable images similar to the CIFAR-10 dataset.
