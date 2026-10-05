# Convolutional Neural Networks

 <img src="/assets/images/1.gif" alt="Illustration representing cnn" style="width:100%; height:auto;" />

A practical and structured guide to understanding, implementing, and evaluating Convolutional Neural Networks (CNNs) for computer vision tasks.

This repository follows a progressive learning path that begins with the fundamental concepts behind CNNs and advances toward framework-based implementation using TensorFlow, Keras, and PyTorch. The final module applies these concepts to an end-to-end image classification project using the MNIST or CIFAR-10 dataset.

The repository is organized with a software engineering mindset, emphasizing maintainable code, reproducible experiments, modular model design, clear documentation, and practical evaluation.

## Learning Objectives

By completing this repository, you will be able to:

- Explain why CNNs are effective for image-based problems.
- Understand convolution operations and feature extraction.
- Work with convolutional layers, filters, kernels, and feature maps.
- Understand padding, stride, and receptive fields.
- Apply pooling techniques for spatial dimensionality reduction.
- Build CNN architectures using Keras and TensorFlow.
- Build CNN architectures using PyTorch.
- Apply regularization techniques to reduce overfitting.
- Use data augmentation to improve model generalization.
- Train and evaluate CNN models on image classification datasets.
- Analyze model performance using relevant evaluation metrics.
- Design CNN experiments using maintainable and reproducible engineering practices.

## Repository Structure

### 1: Introduction to Convolutional Neural Networks

Introduces the architecture, purpose, and core principles of Convolutional Neural Networks.

<img src="/assets/images/2.gif" alt=" cnn architecture" style="width:100%; height:auto;" />

Topics include:

- Limitations of fully connected networks for image data.
- CNN architecture.
- Local connectivity.
- Weight sharing.
- Feature extraction.
- Feature maps.
- Receptive fields.
- CNNs in computer vision applications.

### 2: Convolutional Layers and Filters

Explains how convolutional layers detect meaningful patterns in images.


 <img src="/assets/images/3.gif" alt="Illustration representing cnn" style="width:100%; height:auto;" />
 
Topics include:

- Convolution operations.
- Kernels and filters.
- Stride.
- Padding.
- Feature-map generation.
- Edge and texture detection.
- Multi-channel image processing.
- Output dimension calculations.
- Parameter estimation for convolutional layers.

### 3: Pooling Layers and Dimensionality Reduction

Covers pooling operations and their role in reducing spatial dimensions.


 <img src="/assets/images/4.png" alt="Illustration representing cnn" style="width:100%; height:auto;" />

Topics include:

- Max pooling.
- Average pooling.
 Global average pooling.
- Spatial dimensionality reduction.
- Computational efficiency.
- Translation tolerance.
- Information preservation.
- Effects of pooling on model performance.

### 4: Building CNN Architectures with Keras and TensorFlow

Demonstrates how to design, train, and evaluate CNN models using TensorFlow and Keras.

 <img src="/assets/images/7.gif" alt="Illustration representing cnn" style="width:100%; height:auto;" />

Topics include:

- Defining CNN architectures.
- Convolutional and pooling layers.
- Flattening and fully connected layers.
- Model compilation.
- Loss functions and optimizers.
- Training and validation workflows.
- Callbacks and checkpointing.
- Model evaluation.
- Saving and loading trained models.

### 5: Building CNN Architectures with PyTorch

Introduces CNN implementation using PyTorch.

Topics include:

- PyTorch tensors.
- Dataset and DataLoader abstractions.
- Custom neural network modules.
- Convolutional layers.
- Pooling layers.
- Forward passes.
- Training loops.
- Backpropagation and optimizer steps.
- GPU acceleration.
- Saving and restoring model checkpoints.

### 6: Regularization and Data Augmentation

Explores techniques for improving model generalization and controlling overfitting.

Topics include:

- Overfitting and underfitting.
- Dropout.
- Weight decay.
- Batch normalization.
- Early stopping.
- Learning-rate scheduling.
- Image rotation and translation.
- Flipping and cropping.
- Image scaling.
- Training-time augmentation.
- Validation and test-data integrity.

### 7: CNN Project — Image Classification

Applies the concepts covered throughout the repository to a complete image classification project using MNIST or CIFAR-10.

The project includes:

- Dataset loading and preparation.
- Image normalization.
- Model architecture design.
- CNN training.
- Validation and test evaluation.
- Performance visualization.
- Confusion-matrix analysis.
- Inspection of misclassified examples.
- Regularization and augmentation experiments.
- Model comparison and documentation.

## Technology Stack

- Python
- TensorFlow
- Keras
- PyTorch
- NumPy
- Matplotlib
- scikit-learn
- Jupyter Notebook

## Repository Structure

```text
.
├── README.md
├── requirements.txt
├── day-01-cnn-introduction/
│   └── ...
├── day-02-convolutional-layers/
│   └── ...
├── day-03-pooling-and-dimensionality-reduction/
│   └── ...
├── day-04-cnn-with-tensorflow-keras/
│   └── ...
├── day-05-cnn-with-pytorch/
│   └── ...
├── day-06-regularization-and-augmentation/
│   └── ...
└── day-07-cnn-image-classification-project/
    └── ...
```

> The directory structure may evolve as the project grows. The objective is to keep learning material, reusable components, experiments, and project artifacts clearly separated.

## Prerequisites

Recommended prerequisites include:

- Intermediate Python programming knowledge.
- Familiarity with functions, classes, modules, and virtual environments.
- Basic understanding of NumPy arrays.
- Introductory knowledge of linear algebra.
- Basic understanding of neural networks and gradient-based optimization.
- Familiarity with Git and command-line workflows.

Prior experience with TensorFlow, Keras, or PyTorch is helpful but not required.

## Getting Started

### 1. Clone the repository

```bash
git clone <repository-url>
cd convolutional-neural-networks
```

### 2. Create a virtual environment

```bash
python -m venv .venv
```

Activate the environment on macOS or Linux:

```bash
source .venv/bin/activate
```

Activate the environment on Windows:

```bash
.venv\Scripts\activate
```

### 3. Install dependencies

```bash
pip install -r requirements.txt
```

If a requirements file is not available, install the primary dependencies manually:

```bash
pip install numpy matplotlib scikit-learn tensorflow torch torchvision jupyter
```

### 4. Start Jupyter Notebook

```bash
jupyter notebook
```

Open the notebooks in order, starting with the CNN introduction and continuing through the final image classification project.

## Recommended Learning Workflow

For each module:

1. Review the theoretical concepts.
2. Execute the accompanying notebook or script.
3. Inspect tensor shapes and intermediate outputs.
4. Modify model and training parameters.
5. Compare the impact of different architectures.
6. Track training and validation metrics.
7. Document observations and implementation decisions.
8. Refactor reusable logic into maintainable modules.

The repository is designed to encourage understanding rather than simply executing predefined notebooks.

## CNN Design Considerations

When designing a CNN, consider the following:

- Input image dimensions and number of channels.
- Number of convolutional filters.
- Kernel size.
- Stride and padding.
- Pooling strategy.
- Number of convolutional blocks.
- Activation functions.
- Normalization strategy.
- Dropout and other regularization methods.
- Number of parameters.
- Training and inference performance.
- Risk of overfitting.

A deeper or wider model is not automatically better. Architecture complexity should be aligned with dataset size, task difficulty, hardware availability, and expected deployment requirements.

## Model Evaluation

Model performance should be evaluated using more than a single accuracy value.

Relevant metrics and analysis techniques include:

- Training loss.
- Validation loss.
- Test loss.
- Training and validation accuracy.
- Precision.
- Recall.
- F1-score.
- Confusion matrix.
- Per-class accuracy.
- Misclassified-image analysis.
- Inference latency.
- Model size and resource consumption.

For MNIST, accuracy is often a useful baseline metric. For CIFAR-10, class-level performance, confusion patterns, and generalization behavior should also be reviewed.

## Engineering Practices

This repository follows practical machine learning engineering principles:

- Keep training, validation, and test data separate.
- Avoid data leakage during preprocessing and augmentation.
- Use deterministic seeds where reproducibility is required.
- Track model configuration and hyperparameters.
- Save model checkpoints at meaningful training intervals.
- Keep datasets and generated artifacts out of version control.
- Use modular functions and classes instead of duplicated code.
- Validate tensor dimensions at model boundaries.
- Document assumptions and experimental results.
- Separate exploratory notebooks from reusable production-oriented code.
- Prefer explicit configuration over hard-coded training parameters.

## Example CNN Workflow

A typical CNN training workflow consists of:

```text
Load dataset
    ↓
Normalize and preprocess images
    ↓
Split data into training, validation, and test sets
    ↓
Define CNN architecture
    ↓
Compile or configure the model
    ↓
Train the model
    ↓
Evaluate validation performance
    ↓
Tune architecture and hyperparameters
    ↓
Evaluate on the test set
    ↓
Analyze predictions and errors
    ↓
Save the trained model
```

## Potential Extensions

Possible future improvements include:

- Implementing convolution operations from scratch using NumPy.
- Visualizing learned filters and intermediate feature maps.
- Adding transfer learning with pretrained architectures.
- Experimenting with ResNet, VGG, or MobileNet.
- Adding batch normalization and advanced regularization.
- Comparing CPU and GPU training performance.
- Introducing experiment tracking.
- Adding automated unit tests for preprocessing and model components.
- Creating a command-line training interface.
- Serving the trained model through a REST API.
- Containerizing the inference service with Docker.
- Adding continuous integration and automated quality checks.
- Deploying the model to a cloud or edge environment.

## Contributing

Contributions are welcome. When contributing to this repository:

1. Create a dedicated feature branch.
2. Keep each change focused and appropriately scoped.
3. Follow the existing naming and directory conventions.
4. Update documentation when behavior or structure changes.
5. Validate notebooks and scripts before opening a pull request.
6. Avoid committing datasets, credentials, checkpoints, and generated files.
7. Include a clear explanation of the problem solved or improvement introduced.

## License

This project is intended for educational and experimental purposes. Add an appropriate open-source license, such as the MIT License, before distributing the repository publicly.

## Author

Developed as a practical learning repository for building strong foundations in Convolutional Neural Networks, computer vision, and machine learning engineering.


