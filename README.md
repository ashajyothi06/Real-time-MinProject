"# MINI-PROJECT" 


 ## PROJECT NAME:

#### Human Action Recognition from Depths Maps and Postures Using Deep Learning

## ABOUT PROJECT:

The project implements real-time human activity recognition using depth maps and postures with deep learning. It leverages OpenCV for video processing and a pre-trained ResNet-34 model for action recognition. Frames are captured from a video file or webcam, resized, and stored in a fixed-length queue. Once the queue is full, frames are processed into a blob format and passed through the model to predict the activity. The predicted activity is displayed on each frame in real-time. This system can recognize various human actions, enhancing applications like surveillance and human-computer interaction.
### Technologies and libraries Used:

## Technologies:
Python
ONNX
ResNet-34 model
## Libraries:
OpenCV
NumPy
argparse
imutils
deque (from collections)

## STEPS OVERVIEW:
1.Open Command Prompt/Terminal
2.Clone the Repository
3.Navigate to the Repository Directory
4.Navigate to the Directory Containing Harde.py
5.Install Required Packages: pip install -r requirements.txt
6.Run Harde.py

## PROJECT OVERVIEW:

Here's a detailed working procedure of your human activity recognition:
## Import Libraries:
 Essential libraries such as OpenCV, argparse, and numpy are imported to handle video processing, argument parsing, and numerical operations.
## Argument Parsing: 
Command-line arguments are parsed to get the model path, class labels file, and an optional input video file.
## Load Resources:
 The class labels are read from the specified file and stored in a list. The human activity recognition model is loaded using OpenCV’s cv2.dnn.readNet.
## Initialize Frame Queue:
 A deque is initialized with a fixed length to store the frames required for activity recognition.
## Access Video Stream:
 The video stream is accessed either from the specified video file or the webcam.
## Frame Processing: 
Each frame is read, resized for faster processing, and added to the frame queue.
Check Queue: If the queue is not yet filled to the required sample duration, the loop continues to process and add frames.
## Blob Construction:
 Once the queue is filled, a blob is constructed from the frames using cv2.dnn.blobFromImages and adjusted to match the model's input requirements.
## Model Prediction:
 The blob is passed through the network to obtain activity recognition predictions, and the predicted activity label is determined.
## Display Results:
 The predicted activity is displayed on the frames in real-time, and the annotated frames are shown in a window. The process continues until the 'q' key is pressed to exit the loop.

## Results Obtained
 ![Screenshot 2024-06-21 151430](https://github.com/user-attachments/assets/450179ad-d508-4e18-aa50-548d90a4a91f)
![Screenshot 2024-06-21 151616](https://github.com/user-attachments/assets/d5e2f0cc-1800-42b9-9cc4-4120fe9b49cb)
![Screenshot 2024-06-21 151802](https://github.com/user-attachments/assets/7ea439c1-ede6-4e25-9008-fbea8c5844fa)
![Screenshot 2024-06-21 152223](https://github.com/user-attachments/assets/de5df6c6-5c8a-442d-a4dc-a77706f33463)
![Screenshot 2024-06-21 152706](https://github.com/user-attachments/assets/7a0f45fd-1696-4c98-9644-7e85b8a6ae7b)
