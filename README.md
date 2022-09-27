# uSAR: UAV Based Edge-Enabled Human Detection System for Search and Rescue Operations in Disasters Management
## ✯ Introduction
* UAV can be used in wide range of application like surveillance, delivery, entertainment, warfare, person tracking , etc.
* Person detection in the disaster-hit area is essential in search and rescue operation in disaster management.
* Drones have been widely used in disaster relief because of their small size and ability to operate in various environments.
* Thus, UAV based automatic human detection is very effective for disaster relief response.

## ✯ Objective
* To built a human detection system for search and rescue operations in disasters management.
* To create an object detection model able to detect person in drone imagery.
* Optimize the model for edge inference.

## ✯ Proposed Solution
<img width="977" alt="Screenshot 2022-09-27 at 1 33 16 PM" src="https://user-images.githubusercontent.com/54806252/192469255-9924836d-7a5c-47e4-9f65-a7e33d579d8b.png">

## ✯ Dataset Acquisition
<img width="686" alt="Screenshot 2022-09-27 at 1 39 20 PM" src="https://user-images.githubusercontent.com/54806252/192470607-f873770e-cc8a-48d4-b432-f4f7068031b4.png">

* The dataset used is SARD Dataset . 
* It contains images of person in diverse terrain and backgrounds with different classes such as running, walking, standing, sitting, or lying down. 
* The dataset was split in training and testing data with split size of 0.2. 
* The training set had 1534 images containing 6 classes of activities and testing set had 387 images

## ✯ Proposed Detection Model
* The pre-trained EfficentDet Lite-4 model is fined-tuned on the dataset.
* EfficientDet-Lite object detection models have EfficientNet Lite backbone with BiFPN feature extractor, shared box predictor and focal loss.
* They are trained on COCO 2017 dataset, and optimized for the TensorFlow Lite (TFLite) version, which are specifically designed for performance on mobile CPU, GPU, and EdgeTPU.

## ✯ Results Demonstration
<img width="1065" alt="Screenshot 2022-09-27 at 1 45 53 PM" src="https://user-images.githubusercontent.com/54806252/192471953-0f9c47f6-f67e-4b53-9512-339294e6e293.png">
<img width="1261" alt="Screenshot 2022-09-27 at 1 46 38 PM" src="https://user-images.githubusercontent.com/54806252/192472109-8ba959fc-750a-4de7-bf6c-1cd702ada650.png">
