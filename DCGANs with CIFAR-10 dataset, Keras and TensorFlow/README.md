Generative Adversarial Network (GAN) on CIFAR-10

Overview

This project implements a Generative Adversarial Network (GAN) to generate images based on the CIFAR-10 dataset. The GAN consists of a generator and a discriminator trained adversarially to improve the quality of generated images over time.

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
