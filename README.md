# Brain Tumor Classifier using VGG16

This project implements a brain tumor classifier using TensorFlow and Keras, leveraging the VGG16 pre-trained model for image classification. The classifier is designed to distinguish between MRI images with and without brain tumors.

## Table of Contents

- [Project Overview](#project-overview)
- [Installation](#installation)
- [Dataset](#dataset)
- [Model Architecture](#model-architecture)
- [Results](#results)
- [Contributing](#contributing)
- [License](#license)

## Project Overview

The brain tumor classifier uses the VGG16 model pre-trained on ImageNet, fine-tuned for binary classification of MRI images. The project includes data preprocessing, augmentation, training, evaluation, and visualization of results.

## Installation

1. **Clone the repository:**
    ```bash
    git clone https://github.com/arnnv/brain-tumor-detection.git
    cd brain-tumor-classifier
    ```

2. **Install required dependencies:**
    ```bash
    pip install -r requirements.txt
    ```

## Dataset

The [dataset](https://www.kaggle.com/datasets/navoneel/brain-mri-images-for-brain-tumor-detection/data) should be structured as follows:

```
brain_tumor_dataset/
├── yes/
└── no/
```

## Model Architecture

The classifier uses the VGG16 model with custom dense layers for fine-tuning:
- Base model: VGG16 with pre-trained ImageNet weights (excluding top layers).
- Custom layers: Flatten, Dense (512 units, ReLU activation), Dropout (0.2), Dense (1 unit, sigmoid activation).

## Results

The model achieves 90% accuracy in classifying MRI images with and without brain tumors. Training and validation performance metrics are visualized using Matplotlib.

## Contributing

Contributions are welcome! Please fork the repository and submit a pull request for any enhancements or bug fixes.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.