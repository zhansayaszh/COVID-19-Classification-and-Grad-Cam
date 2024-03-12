# COVID-19-Classification-and-Grad-Cam

## Introduction
The importance of Covid-19 classification and detection in machine learning cannot be overstated. Utilizing advanced algorithms, 
such as deep learning, enables swift and accurate identification of Covid-19 cases. 
This early detection aids in timely interventions, 
containment efforts, and resource allocation. Moreover, machine learning contributes to predictive modeling, assisting in forecasting disease spread and guiding public health policies.
#
In this project the binary dataset was built then ResNet was applied for classification of COVID-19. Then only infected images were taken for visualization using Grad-CAM, 
which finaly shows heat-map with infection. 
## Setup

`pip install imutils`
#
`pip install image-classifiers==1.0.0b1`

## Requirements
- tensorflow
- keras
- scikit-learn
- imutils
- matplotlib
- pandas
- numpy
- opencv-python
  
## Dataset
### covid19_radiography_dataset
The COVID-19 Radiography Dataset is a collection of chest X-ray and CT scan images that have been compiled to aid in the research and development of machine learning models for detecting COVID-19. 
The dataset contains COVID(3616 images) and NORMAL(3616 images), but 500 samples from each were taken for building our dataset.
![image](https://github.com/zhansayaszh/COVID-19-Classification-and-Grad-Cam/assets/28733943/e90ed9b3-97de-4045-911f-f698a8a9499c)

## Model
Resnet34 is used for classification.
![image](https://github.com/zhansayaszh/COVID-19-Classification-and-Grad-Cam/assets/28733943/ee657d28-90cc-4979-ba5f-e210a653ea85)

## Results
Our model reached 0.9 accuracy in classification.
![image](https://github.com/zhansayaszh/COVID-19-Classification-and-Grad-Cam/assets/28733943/34199301-4c0a-4b22-8c4e-e2defd3a59ef)
![image](https://github.com/zhansayaszh/COVID-19-Classification-and-Grad-Cam/assets/28733943/5509d857-6404-443e-8b8b-f8be143606db)

## GradCam
The heat-map is shown by visualizing the final convolutional layer of ResNet34.
![image](https://github.com/zhansayaszh/COVID-19-Classification-and-Grad-Cam/assets/28733943/ba3d7ab2-5731-46d7-8b64-516dc72b6972)
