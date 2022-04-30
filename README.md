![background](https://user-images.githubusercontent.com/67295703/164965154-f5422c0a-e565-4328-972b-030aac5dfbb0.png)
# Distracted drivers
Image classification of distracted drivers.

[Link to the full notebook](https://nbviewer.org/github/CyperStone/distracted-drivers/blob/main/distracted_drivers.ipynb)

## Project Overview
* Loaded, analyzed and performed augmentation on dataset with images of distracted drivers
* Created a CNN model that classifies (Accuracy ~ 98.22%) drivers behaviour behind the wheel:
![alt text](https://github.com/CyperStone/distracted-drivers/blob/main/visualization/confusion_matrix.png)

## Technologies
* Python Version: 3.9
* Packeges: tensorflow, scikit-learn, pandas, numpy, cv2, matplotlib, plotly

## About the Dataset
* Source: https://www.kaggle.com/competitions/state-farm-distracted-driver-detection
* The dataset contains 22424 labeled images (640x480) of drivers and csv file with info about each picture
* Drivers behavior is divided to 10 (quite balanced) classes. Classes overview:
 ![alt text](https://github.com/CyperStone/distracted-drivers/blob/main/visualization/classes.png)
 
## Model architecture and performance:
 * Trained custom CNN model with the following architecture:
 
 <a href="url"><img src="https://github.com/CyperStone/distracted-drivers/blob/main/visualization/model_architecture.png" width="500" height="900"></a>
 * Model misclassified only 80 images out of 4485 in the test set (many of them would be challenging to distinguish even for people) and reached the following metrics:
 
 ![alt text](https://github.com/CyperStone/distracted-drivers/blob/main/visualization/results.png)
