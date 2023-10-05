# TensorFlow GPU Compatibility Checker and Performance Tester

This Python script is designed to serve two main purposes:

1. **GPU Compatibility Checker:** It checks if TensorFlow is working correctly on your GPU and provides information about your GPU setup. It also suppresses unnecessary warnings to ensure a smooth experience.

2. **Performance Tester:** It demonstrates the significant performance advantage of GPU-enabled TensorFlow over the CPU by training a Convolutional Neural Network (CNN) model on the CIFAR-10 dataset for image classification. The script compares multiple metrics and provides various visualizations to help you understand the difference in performance between CPU and GPU.

## Features

### GPU Compatibility Check

The script performs the following tasks to check GPU compatibility:

- Suppresses warnings related to CUDA/CuDNN/TensorFlow to enhance the user experience.
- Displays information about Python, Driver, and TensorFlow versions.
- Sets the GPU as the default device if available.
- Checks for the presence of GPUs and lists local devices.

### Performance Testing

The script demonstrates GPU superiority by training a CNN model on the CIFAR-10 dataset and provides various metrics and visualizations:

- **Training Time Comparison:** Compares training times between CPU and GPU for different batch sizes.
- **Combined Metrics Comparison:** Compares accuracy, recall, precision, specificity, and AUC-ROC for CPU and GPU.
- **Class-Specific Accuracy:** Calculates class-specific accuracy scores for each class and visualizes them.
- **Class-Specific Accuracy Heatmap:** Provides a heatmap visualization of class-specific accuracy scores.
- **Class-Specific Accuracy Summary:** Summarizes class-specific accuracy scores, ranks classes, and calculates the weighted average.

## Dependencies

Before running this script, make sure you have the following prerequisites installed:

- Python
- TensorFlow
- TensorFlow Datasets
- TensorFlow Keras
- Scikit-Learn
- NumPy
- Matplotlib
- Seaborn
- tqdm
- Pandas

You can install these dependencies using pip with the following command:

```bash
pip install tensorflow tensorflow-datasets scikit-learn numpy matplotlib seaborn tqdm pandas

This youtube video leads to a docker image which is very well suited for running tensorflow with an nvidia GPU:
https://youtu.be/YozfiLI1ogY?si=Sb6q807ILbPNQiIc

You may also be able to just find the image by searching the container database:
thegeeksdiary/tensorflow-jupyter-gpu:latest
