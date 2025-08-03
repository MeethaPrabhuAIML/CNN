# CNN

## Project Overview: Animal Image Classifier
This project showcases the development and deployment of a Convolutional Neural Network (CNN) designed to classify images of animals into one of ten categories. Leveraging deep learning and a rich dataset of real-world images, the model is trained to recognize animals such as dogs, cats, elephants, and more with high accuracy.

The final model is deployed using Gradio, enabling an easy-to-use web interface where users can upload animal images and receive real-time classification results.

## Dataset: Animals-10
The dataset used is the popular Animals-10 collection, sourced from Kaggle. It consists of over 26,000 images categorized into ten animal classes: Dog, Horse, Elephant, Butterfly, Chicken, Cat, Cow, Sheep, Spider, and Squirrel.

Images are diverse in background, lighting, and pose, making the classification task realistic and challenging. The dataset is loaded and processed with appropriate resizing, normalization, and split into training, validation, and test sets.

## Preprocessing
All images are resized to a uniform shape to ensure compatibility with the CNN. Pixel values are normalized to a [0, 1] scale to facilitate faster convergence during training. Labels, originally in Italian, are mapped to English for clarity. Data is divided into training, validation, and test sets using built-in utilities to ensure consistent sampling and reproducibility.

## Model Architecture
The model is a custom-built CNN comprising multiple convolutional and pooling layers, followed by fully connected layers with dropout regularization. It uses standard activation functions and optimization techniques to learn hierarchical features from the input images.

The architecture is simple yet effective, balancing performance and training speed. It is trained using categorical cross-entropy loss and evaluated using classification accuracy.

## Training and Evaluation
The model is trained over multiple epochs with early stopping to prevent overfitting. Performance is monitored on both training and validation datasets.

Upon evaluation on the test set, the model achieves an accuracy of 83%, demonstrating strong generalization ability. A confusion matrix is used to analyze prediction distribution across different classes, helping identify areas for potential improvement.

## Deployment with Gradio
To make the model accessible and interactive, a Gradio-based web interface is developed. Users can upload any animal image and instantly get a prediction of the animal class.

The deployment allows real-time testing of the model and can be shared or hosted online without requiring users to install any software or understand the underlying code.

## Key Highlights
Real-world image classification with a custom CNN

Robust performance across 10 animal categories

Interactive deployment using Gradio

Achieves over 83% accuracy on test data

Includes evaluation tools like confusion matrix and visual prediction outputs

