# Mood_Detection_Using_Facial_Expression
# 😊 Mood Detection Using Facial Expression and Deep Learning

This research project focuses on building a real-time facial mood detection system using Convolutional Neural Networks (CNNs). The system classifies emotions into five categories—Happy, Sad, Angry, Surprise, and Neutral. Uses Streamlit for its user interface.

## Features
- Real-time webcam & image upload support
- CNN model trained on FER-2013 dataset
- Text-to-Speech feedback using `pyttsx3`
- MySQL database integration for record storage
- Session state tracking and UI refresh functionality
- User-friendly web UI built with Streamlit

## Model Architecture
The model includes:
- Conv2D, MaxPooling2D, Dropout, and BatchNorm layers
- Final SoftMax layer for classification into 5 classes

I have added the Architecture of model i used for my research as **CNN Architecture.png** in this github repository.

## Application Flow
Step-by-Step Flow: 
1. Image Input Interface - Users can either capture a live image using the webcam or upload an existing photo. 
The interface is built using Streamlit for easy interaction. 
2. Face Detection - OpenCV converts the image to grayscale and detects faces using Haar Cascade. If no 
or multiple faces are detected, the user is prompted to retry. 
3. Preprocessing - The detected face is resized to 48×48 pixels and normalized. It is then reshaped to 
match the CNN input format. 
4. Error Handling - The system notifies the user if lighting is poor or no valid face is found.  
5. Emotion Prediction - The pre-processed image is passed to a trained CNN model. It predicts one of five 
emotions along with a confidence score. 
6. Text-to-Speech Feedback - The detected emotion is spoken aloud using pyttsx3. This helps with accessibility and 
real-time interaction. 
7. Save Result Prompt - After prediction, the user is asked if they want to save the result. If yes, a form appears 
to collect user details. 
8. Personal Details Form - Users enter their Name, Age, and Gender. These details are stored along with the 
emotion prediction. 
9. Database Logging -All information is added into a MySQL table named emotion records. This happens 
before showing the summary.[13] 
10. Summary Display -A summary page shows user details, detected emotion, and face image. A button 
allows printing or downloading the result. 

I have added the application flow of my mood detection system as **Application Flow.png** in this github repository.

## Published Research
- Journal: IRJMETS – International Research Journal of Modernization in Engineering Technology and Science
- Volume 07, Issue 06, June 2025
- DOI: [https://www.doi.org/10.56726/IRJMETS80333]

I have added the my published reasech paper whole pdf as **Published research Paper.pdf** in this github repository.

## Author 
Miss. Manisha Raghoba Agarwadekar
Student, 
Dept. of Information Technology
University of Mumbai, Sindhudurg Sub Campus

## ⚠️ Disclaimer
Due to academic privacy, the complete code and model are not included in this repository. For further details or collaboration, feel free to contact the author via LinkedIn.
