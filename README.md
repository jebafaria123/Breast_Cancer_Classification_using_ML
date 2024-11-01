# Image Classification Using ResNet101

## Overview
The goal of this project is to classify overlayed images into three categories: **benign**, **malignant**, and **normal**. Utilizing transfer learning with the ResNet101 architecture, this project addresses challenges in image classification by leveraging pre-trained models and optimizing the training process for accuracy and efficiency.

## Key Methodology

### 1. Data Collection and Preprocessing
Data preprocessing is essential for preparing the images for classification. Key tasks involved include:
- **Image Resizing:** Ensuring all images are resized to the input dimensions required by the ResNet101 model.
- **Normalization:** Normalizing pixel values to improve model training efficiency and performance.
- **Data Augmentation:** Applying transformations (like rotation, flipping, and zooming) to increase the diversity of the training dataset, thus reducing overfitting.

**Data Preprocessing Workflow:**
- Collect overlayed images from specified directories for each category.
- Resize and normalize images before feeding them into the model.

### 2. Data Splitting
The dataset is divided into training, validation, and test sets to effectively evaluate the model's performance. The splitting process maintains the distribution of classes across these sets, ensuring a representative evaluation of the model's capabilities.

### 3. Model Selection
The project employs the ResNet101 architecture, a deep residual network known for its effectiveness in image classification tasks. The model is fine-tuned using transfer learning, where weights from a pre-trained model are adjusted to fit the new dataset, thereby leveraging learned features from previous training.

### 4. Model Training
Training involves:
- Utilizing the training set to teach the model how to classify images.
- Monitoring training and validation loss/accuracy to prevent overfitting through techniques such as early stopping.

### 5. Model Evaluation
The performance of the trained model is rigorously evaluated using various metrics:
- **Accuracy:** The proportion of correctly predicted images.
- **Confusion Matrix:** Visual representation of the model’s predictions against the true labels, highlighting areas of confusion.
- **Classification Report:** Metrics including precision, recall, and F1-score for each class to assess the model’s predictive capabilities.

Models are compared based on these performance metrics to determine the effectiveness of the ResNet101 architecture in classifying overlayed images.

## Results
Upon completion of training and evaluation, the results include:
- Graphs depicting training and validation accuracy and loss over epochs.
- A saved model file (`Resnet_fineTuning.pth`) for future predictions.
- A summary of classification metrics detailing the model's performance.

The findings confirm the model's capability to classify overlayed images with high accuracy, demonstrating the effectiveness of transfer learning in this context.
