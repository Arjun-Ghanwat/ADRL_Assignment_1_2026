# ADRL_Assignment_1_2026
# ADRL Assignment 1

My implementations for the Advanced Deep Representation Learning assignment, using PyTorch. The notebooks cover generative models for satellite images, ECG signals, and 3D point clouds.

- `adrl-assignment-q1.ipynb` — f-GAN, BiGAN, WGAN-GP, and custom Fréchet Feature Distance on 13-band EuroSAT images.
- `adrl-assignment-q2.ipynb` — cyclical beta-VAE, latent traversal, spherical VQ-VAE, and StarGAN on MIT-BIH ECG signals.
- `adrl-assignment-q3.ipynb` — Sinkhorn autoencoder and sliced Wasserstein autoencoder. This version uses ModelNet40; the assignment PDF specifies Human3.6M.

The notebooks include training outputs, plots, and numerical checks, with random seeds set to 2026.

To run them, install `torch`, `numpy`, `matplotlib`, `rasterio`, and `wfdb`. Open the notebooks in Kaggle or Jupyter, update the dataset and output paths, and run the cells in order. A GPU is helpful for training. Q1.4 uses the checkpoint produced by Q1.3.

For the course submission, the three parts still need to be combined into one notebook with the required written explanations.
