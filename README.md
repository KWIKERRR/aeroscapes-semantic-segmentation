# Image Segmentation with TensorFlow Garden
This repository contains a comprehensive implementation of a deep learning model for image segmentation using TensorFlow Garden. The model is designed for the task of segmenting images into different classes.

## Aeroscapes Semantic Segmentation Dataset
The code is tailored for the Aeroscapes dataset, a challenging benchmark for semantic segmentation tasks. The dataset consists of images captured in outdoor environments with diverse scenes. It is annotated with pixel-wise labels for 12 different classes, including road, building, vegetation, and more. The dataset can be accessed [here](https://www.kaggle.com/datasets/kooaslansefat/uav-segmentation-aeroscapes/data).
### Dataset Structure
 - ImageSets
     - trn.txt (list of training file names)
     - val.txt (list of validation file names)
- JPEGImages
  
     Image files for training, validation, and testing
  
- SegmentationClass
  
     Segmentation mask files for training, validation, and testing

## Features
### Data Loading and Preprocessing
The code includes a robust data loading and preprocessing pipeline. It supports loading images and corresponding segmentation masks from specified file paths, and the images are resized to a standardized size.

### TFRecord Generation
To efficiently handle large datasets, the script includes functionality to convert the dataset into TFRecord files. TFRecords are a recommended format for TensorFlow, providing improved performance during training.

### Custom Data Generator
A custom data generator class is implemented to handle the loading and preprocessing of images and masks in batches. This ensures memory-efficient training and allows for easy integration with TensorFlow's data input pipelines.

### Model Configuration
The model architecture and training parameters can be easily configured using a set of variables. The script supports a variety of options, including the choice of a pre-trained backbone and the number of classes for segmentation.

### Training and Evaluation
The training process is managed with TensorFlow's TF-Agents library. The script includes functionality to run training and evaluation loops, leveraging distributed training across multiple GPUs or TPUs if available.

### Visualization
The code provides visualization tools to display input images, true segmentation masks, and predicted masks during or after the training process. This aids in understanding the model's performance.

## Dependencies
This code depends on the following librairies :
 - tensorflow >= 2.9.2
 - tf-models-official

## Customization
Feel free to customize the script according to your specific use case. You can adjust hyperparameters, experiment with different backbones, or modify the data loading pipeline to suit your dataset.

## Contributing
Contributions are welcome! If you find any issues or have suggestions for improvements, please open an issue or submit a pull request.

Happy coding !
