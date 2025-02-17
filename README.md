# Heart-Detection-in-X-ray-Images-Using-VGG16
This project focuses on developing a deep learning model for detecting the heart in X-ray images. The model is built on top of the VGG16 architecture and is trained to predict the coordinates of bounding boxes that encapsulate the heart. 

### Features 
X-ray images were loaded and preprocessed from a directory. VGG16 architecture with custom fully connected layers has been deployed for bounding box regression. Various image transformations have been applied to enhance the robustness of the model. The predicted and actual bounding boxes have been overlayed on the X-ray images for visual validation of the model's performance.

### Dataset
The dataset consists of X-ray images with annotated bounding boxes for the heart region from the RSNA Pneumonia Detection Challenge in Kaggle. The images are organized in a directory structure and are in .npy format. Each image has an associated bounding box that specifies the coordinates (x_min, y_min, x_max, y_max).

### Model Architecture
The model is based on the VGG16 architecture, a widely-used convolutional neural network. The classifier part of the VGG16 model is modified to include custom fully connected layers for bounding box regression.

### Training
The model is trained using the Adam optimizer and the Mean Squared Error (MSE) loss function, which is appropriate for regression tasks. The training loop iterates through the dataset, computes the loss, performs backpropagation, and updates the model weights. 

### Evaluation
The model's performance is evaluated using a validation set. The predicted bounding boxes are compared with the ground truth bounding boxes, and visualizations are generated to assess the accuracy of the predictions.

### Visualization
The project includes a script to visualize the results by overlaying the predicted and ground truth bounding boxes on the X-ray images. This helps in qualitatively evaluating the model's performance.

![Heart_Detection](https://github.com/vaibhavmallya98/Heart-Detection-in-X-ray-Images-Using-VGG16/assets/45683079/1fb3a5f7-87db-4bce-bcf4-7e137501809e)
