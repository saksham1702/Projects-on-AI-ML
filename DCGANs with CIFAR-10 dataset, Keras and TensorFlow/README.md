# Generative Adversarial Network (GAN) on CIFAR-10

## Project Overview

This project implements a **Generative Adversarial Network (GAN)** to generate images based on the **CIFAR-10** dataset. The GAN consists of two primary components:
- **Generator**: Creates synthetic images from random noise vectors (latent space).
- **Discriminator**: Distinguishes between real and generated images, providing feedback to improve the generator.

The generator and discriminator are trained adversarially, meaning they both compete to improve each other's performance. The training process involves using real CIFAR-10 images and the generated images to refine the models and improve the quality of generated images over time.

## Key Features

- **Batch Training**: Uses both real and generated images for training.
- **Latent Space Sampling**: Generates images from random noise vectors.
- **Loss Tracking**: Tracks the loss for both the generator and discriminator to monitor progress.
- **Periodic Image Visualization**: Regularly visualizes the generated images to track improvements.

## Results

After training for a sufficient number of epochs, the generator should be capable of producing somewhat visually recognizable images that closely resemble those from the CIFAR-10 dataset.

## Potential Issues & Fixes

- Ensure the CIFAR-10 dataset (`X_train`) is loaded correctly.
- Verify that the variables `latent_dim`, `WIDTH_SIZE`, and `HEIGHT_SIZE` are properly defined.
- Use `generator.predict(z)` or `generator.predict_on_batch(z)` consistently for generating images.
- Normalize the generated images correctly before visualization.
