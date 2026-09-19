# ADRL Assignment 1

My implementations for the Advanced Deep Representation Learning assignment, using PyTorch. The notebooks cover generative models for satellite images, ECG signals, and 3D point clouds.

- `adrl-assignment-q1.ipynb` — f-GAN, BiGAN, WGAN-GP, and custom Fréchet Feature Distance on 13-band EuroSAT images.
- `adrl-assignment-q2.ipynb` — cyclical beta-VAE, latent traversal, spherical VQ-VAE, and StarGAN on MIT-BIH ECG signals.
- `adrl-assignment-q3.ipynb` — Sinkhorn autoencoder and sliced Wasserstein autoencoder. This version uses ModelNet40; the assignment PDF specifies Human3.6M.

The notebooks include training outputs, plots, and numerical checks, with random seeds set to 2026.

## Datasets

- **[EuroSAT (Kaggle)](https://www.kaggle.com/datasets/apollo2506/eurosat-dataset)** — Satellite images covering 10 land-use and land-cover classes. Q1 uses the 64×64 TIFF images with all 13 spectral bands.
- **[MIT-BIH Arrhythmia (official PhysioNet site)](https://physionet.org/content/mitdb/1.0.0/)** — Annotated ECG recordings sampled at 360 Hz. Q2 uses one-second windows around normal (N) and premature ventricular contraction (V) beats.
- **[ModelNet40 (Kaggle)](https://www.kaggle.com/datasets/balraj98/modelnet40-princeton-3d-object-dataset)** — 3D object meshes across 40 categories. Q3 samples 256 points from each mesh surface and normalizes them before training.

To run them, install `torch`, `numpy`, `matplotlib`, `rasterio`, and `wfdb`. 

For the course submission, the three parts still need to be combined into one notebook with the required written explanations.
