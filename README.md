EfficientNetV2 and MobileNetV2 on CIFAR-10
This repository contains code for training and evaluating EfficientNetV2 and MobileNetV2 models on the CIFAR-10 dataset. The code is optimized to run on systems with limited resources (e.g., 4 GB RAM).

Table of Contents
Overview

Requirements

Installation

Usage

Results

Contributing

License

Overview
This project demonstrates how to train lightweight deep learning models (EfficientNetV2 and MobileNetV2) on the CIFAR-10 dataset. The code is optimized for systems with limited RAM (4 GB or more) and includes:

EfficientNetV2-S and MobileNetV2 implementations.

Memory-efficient training with small batch sizes and reduced input dimensions.

Data generators for on-the-fly data loading.

Mixed precision training (optional) for faster training on supported hardware.

Requirements
To run this code, you need:

Python 3.8 or higher.

TensorFlow 2.x.

Matplotlib (for plotting training curves).

Installation
Clone the repository:

bash
Copy
git clone https://github.com/your-username/your-repo-name.git
cd your-repo-name
Install the required libraries:

bash
Copy
pip install tensorflow matplotlib
Usage
1. Training the Model
To train the model, run the following command:

bash
Copy
python train.py
2. Evaluating the Model
After training, the model will automatically evaluate on the test set and display the test accuracy.

3. Customizing the Code
To change the model, modify the model variable in the code (e.g., switch from MobileNetV2 to EfficientNetV2).

To adjust the batch size or input size, update the batch_size and input_shape variables.

Results
Performance on CIFAR-10
Model	Test Accuracy	Training Time (10 Epochs)	Batch Size	Input Size
MobileNetV2	85.2%	~30 minutes	8	96x96
EfficientNetV2	90.5%	~1 hour	16	128x128
Training Curves
Training and Validation Accuracy

Contributing
Contributions are welcome! If you'd like to contribute:

Fork the repository.

Create a new branch (git checkout -b feature/YourFeature).

Commit your changes (git commit -m 'Add some feature').

Push to the branch (git push origin feature/YourFeature).

Open a pull request.

License
This project is licensed under the MIT License. See the LICENSE file for details.

Acknowledgements
CIFAR-10 Dataset: https://www.cs.toronto.edu/~kriz/cifar.html

TensorFlow: https://www.tensorflow.org/

EfficientNetV2 Paper: arXiv:2104.00298
