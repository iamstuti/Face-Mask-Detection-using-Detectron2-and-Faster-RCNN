# Face-Mask-Detection-using-Detectron2-and-Faster-RCNN
Performing face detection using Detectron2 and Faster RCNN model by preprocessing &amp; augmenting Kaggle dataset 

### Overview of Detectron2
Detectron2 is a popular PyTorch based modular computer vision model library. The Detectron2 system allows you to plug in custom state of the art computer vision technologies into your workflow.

### Dataset Overview
The Face Mask detection dataset is representative of a small custom object detection dataset that one might collect to construct a custom object detection system. Notably, face mask detection is not a capability available in Detectron2 - we need to train the underlying networks to fit in our custom task.

For this project, I have downloaded the [Face Mask Detection Dataset from Kaggle](https://www.kaggle.com/andrewmvd/face-mask-detection). The dataset is then uploaded to Roboflow. Roboflow is used to select a train/test split for these images. In this project, the default of 70% training, 20% validation, and 10% testing is used as a safe bet.Augmentation of random noise of about (5%). Other settings remains as they were: auto-orient and resize 416x416.

The dataset is then exported in COCO JSON format from Roboflow

You can refer to the README.md inside the zip of our custom dataset exported from Roboflow

### Prerequisites
All the necessary prerequisites are mentioned in the code file.

To get started make a copy of this Colab Notebook. Google Colab provides us with free GPU resources so make sure to enable them by checking Runtime --> Change runtime type --> GPU.

You can refer to the zip for more information about the preprocessing, augmentation applied on the Kaggle Face Detection Kaggle Dataset before exporting it in COCO format.

### Results

Our model makes good predictions showing that it has learned how to identify face masks, faces/people without face masks. Although, it sometimes fails in prediction of "faces with incorrect masks".




