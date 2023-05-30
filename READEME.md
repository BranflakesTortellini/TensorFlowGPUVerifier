This script tests the following:

- It checks if you have TensorFlow (TF) installed and displays the Python and driver versions.
- Sets the GPU as the default device if available and reports the number of physical and logical GPUs detected.
- Verifies the availability of a GPU and displays the number of GPUs available.
- Displays the local devices using TensorFlow.
- Performs a training task using the MNIST dataset and measures the training progress.
- Prints the loss and accuracy information for the specified number of epochs.
- Records the loss and accuracy history during training.
- Calculates the total training time and average time per epoch.
- Plots the loss and accuracy curves.
- Displays the final loss and accuracy values.

Additional notes:

- The script requires compatible versions of CUDA and cuDNN to function properly.
- It demonstrates how to use TensorFlow for training a basic neural network on the MNIST dataset.
- The script provides insights into the training progress and visualizes the model's loss and accuracy trends.
- It serves as a diagnostic tool for checking the availability of GPUs and their utilization in TensorFlow.
- The script helps identify potential compatibility issues related to GPU configuration in TensorFlow setups.
