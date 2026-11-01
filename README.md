# Human-Activity-Recognition
A Python program that uses a pre-trained ResNet-34 deep learning model to recognize human activities from videos or a webcam feed.

# Features
- Recognizes human activities from video
- Supports webcam input
- Uses a pre-trained Deep Learning model
- Can use CUDA GPU acceleration
- Displays the predicted activity on each video frame
- Can save the processed video

**Before running the project, you need to download the pre-trained model: resnet-34_kinetics.onnx**

# How to Run
(replace HAR.py and Actions.txt with the names of your files)

Open a terminal in the project folder and run:<br />
**python HAR.py --model resnet-34_kinetics.onnx --classes Actions.txt**<br />
This will start the Human Activity Recognition application using your webcam.

To analyze a video file, use:<br />
**python HAR.py --model resnet-34_kinetics.onnx --classes Actions.txt --input video.mp4**

To save the processed video, add the --output argument:<br />
**python HAR.py --model resnet-34_kinetics.onnx --classes Actions.txt --input video.mp4 --output output.mp4**
