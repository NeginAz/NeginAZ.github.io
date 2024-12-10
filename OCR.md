---
title: Optical Character Recognition for old writings
---




- Cuneiform script is an ancient writing method used for languages such as Old Persian, Sumerian, and Babylonian.
- The script consists of 37 characters and is associated with inscriptions from the Achaemenid period.
- Due to the limited number of experts in ancient languages and the historical importance of these writings, this research focuses on automating the reading and translation of ancient texts.
- A key objective is to select the most suitable algorithm for data classification, given the scarcity of cuneiform resources.
- The project evaluates different methods, with the best approach being reported.

<h4>Methods</h4>

- Collected and preprocessed a dataset of ancient Persian cuneiform characters from historical inscriptions using image processing -tools like OpenCV for noise reduction and thresholding.
- Extracted character images from inscriptions using template matching algorithms to locate and segment symbols from the background accurately.
- Applied data augmentation techniques (rotation, scaling, translation) using OpenCV to increase dataset size and improve model generalization.
- Generated synthetic data with Autoencoders to create variations of existing characters, enhancing the dataset and mitigating class imbalance.
- Designed and implemented Convolutional Neural Networks (CNN) using TensorFlow/Keras to classify cuneiform characters, optimizing architecture for image recognition tasks.
- Leveraged transfer learning with pre-trained models to boost classification accuracy, adapting models trained on standard datasets to cuneiform character recognition.
- Applied Multi-Layer Perceptron (MLP) networks for character classification and compared their performance with CNN models for baseline evaluation.
- Employed Few-Shot Learning techniques to enable character classification with limited data, improving recognition accuracy on rare symbols.
- Evaluated model performance using metrics such as accuracy, confusion matrices, and loss curves to refine models and identify areas for improvement.
- Developed a complete translation pipeline that integrated character detection and classification to convert ancient Persian cuneiform into modern Persian text.


 <center>
 <div class = "column">
    <img src="https://github.com/user-attachments/assets/97b5d141-325d-4f56-858e-43b7054cbe37" width = "400" position = "relative" align ="center">
 </div>
 </center>

For better classification performance, the dataset was created as images with a black background. Then, similar samples of each character were generated using autoencoders.

  <center>
 <div class = "column">
    <img src="https://github.com/user-attachments/assets/9dc0674e-1b45-42f7-98b5-c04e256c5a18" width = "400" position = "relative" align ="center">
 </div>
 </center>

Various algorithms were used for character classification, but ultimately the images were classified using a CNN (Convolutional Neural Network).

 <center>
 <div class = "column">
    <img src="https://github.com/user-attachments/assets/892cb9c1-c83f-43a2-8c28-0e1f6f238f04" width = "400" position = "relative" align ="center">
 </div>
 </center>


Then, based on locating the coordinates of the page contours, the characters in the text images are identified and translated.

 <center>
 <div class = "column">
    <img src="https://github.com/user-attachments/assets/d4c00812-e4d2-42c8-a00a-c4662b186e8e" width = "400" position = "relative" align ="center">
 </div>
 </center>

By classifying the characters using the designed network, an accuracy of 84% was achieved on the test samples.

 <center>
 <div class = "column">
    <img src="https://github.com/user-attachments/assets/2e5ff432-e57e-4f12-80c9-a03928406e89" width = "400" position = "relative" align ="center">
 </div>
 </center>

