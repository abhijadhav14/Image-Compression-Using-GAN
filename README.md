# Image-Compression-Using-GAN
Autoencoder implementation in PyTorch for image compression with PSNR, SSIM metrics, and visualization. Trainable on custom PNG dataset, the code provides an efficient way to compress images and evaluate reconstruction quality.

Autoencoder for Image Compression:

This repository contains a Jupyter Notebook demonstrating image compression using a simple autoencoder implemented in PyTorch.
The autoencoder is trained on a custom dataset of PNG images.

Dependencies:

PyTorch: Deep learning library for building and training neural networks.
torchvision: PyTorch library for computer vision tasks.
Pillow: Python Imaging Library for opening, manipulating, and saving many different image file formats.
scikit-image: Library for image processing tasks, used for calculating PSNR and SSIM metrics.


Dataset Handling:

Custom dataset class (CustomDataset) is defined to load and preprocess PNG images.
DataLoader is used to efficiently load batches of images during training.


Autoencoder Architecture:

Simple autoencoder architecture is defined in the Autoencoder class, consisting of convolutional and transpose convolutional layers.


Training:

The autoencoder is trained on the specified dataset using mean squared error loss and the Adam optimizer.


Metrics Calculation:

Peak Signal-to-Noise Ratio (PSNR) and Structural Similarity Index (SSIM) are calculated for each compressed image.


Display Images and Metrics:

The notebook includes a function (display_images) to visually compare original and compressed images.
PSNR, SSIM, and Compression Ratio are printed for each image.
Note:

The win_size parameter in SSIM calculation is set dynamically based on the smaller side of the images to avoid errors related to image extent.


How to Use:

Clone the repository.
Provide the path to your custom dataset folder.
Run the notebook to train the autoencoder, display images, and calculate metrics.
