# aeroscapes-semantic-segmentation
Aeroscapes semantic segmentation (12 classes)


## Deep Learning for Image Segmentation with TensorFlow Garden
This repository contains a comprehensive implementation of a deep learning model for image segmentation using TensorFlow. The model is designed for the task of segmenting images into different classes, making it suitable for a variety of applications, such as object detection and scene understanding.

### Features
#### Data Loading and Preprocessing
The code includes a robust data loading and preprocessing pipeline. It supports loading images and corresponding segmentation masks from specified file paths, and the images are resized to a standardized size.

#### TFRecord Generation
To efficiently handle large datasets, the script includes functionality to convert the dataset into TFRecord files. TFRecords are a recommended format for TensorFlow, providing improved performance during training.

##### Custom Data Generator
A custom data generator class is implemented to handle the loading and preprocessing of images and masks in batches. This ensures memory-efficient training and allows for easy integration with TensorFlow's data input pipelines.

#### Model Configuration
The model architecture and training parameters can be easily configured using a set of variables. The script supports a variety of options, including the choice of a pre-trained backbone and the number of classes for segmentation.

#### Training and Evaluation
The training process is managed with TensorFlow's TF-Agents library. The script includes functionality to run training and evaluation loops, leveraging distributed training across multiple GPUs or TPUs if available.

#### Visualization
The code provides visualization tools to display input images, true segmentation masks, and predicted masks during or after the training process. This aids in understanding the model's performance.
