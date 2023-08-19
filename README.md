# Self-Driving-Car-Simulator-Project
A convolutional neural network is trained in this research to imitate a driving style from a simulator. The End to End Learning for Self-Driving Cars publication by NVIDIA is where the CNN architecture utilised in this article is cited.

The objective is to develop and test a CNN model that replicates driving behaviour from a simulator.
The model is trained using only 3 camera views (centre, left, and right) and appropriate steering angles.
The steering angle is the result of the model.

**Data Collection**
The simulator is used to collect the data.
Three laps have been run while the data was being collected, as follows:

In the first lap, making smooth turns and attempting to stay as much as possible in the centre of the queue, one round of data was recorded.
In the second lap, one turn was made with the car going the other way. In actuality, the data that was gathered in the data augmentation stage of the previous round did not require this stage because it was sufficient. The data augmentation has the effect of doubling the amount of data in both ways.
In the third lap, short rides with various patterns were produced from sharp spots to the middle line.

These were used to create the driving log files. 
The Images used to train the data was gotten from the assessment 3 folder in Blackboard.



**Project Pipeline**

The pipeline consists of the following steps:
1. Loading the data
2. Summary of the Dataset & Visual Exploration
3. Data augmentation: Images are cropped to remove unimportant parts. Images are flipped and the steering angles corresponding to them are multiplied by -1 Images Pre-Processing: Here, the picture was only resized.
4. Using Keras to create the CNN Architecture
5. The CNN architecture utilised is displayed below:
    The CNN architecture is taken from a paper on end-to-end learning for autonomous vehicles from NVIDIA. Reference: https://arxiv.org/pdf/1604.07316v1.pdf
6. Saving the Model
Finally, the model is built using the Adam optimizer and Mean Square Error (MSE) loss function.


**Files Submitted**
Submission includes all required files and can be used to run the simulator in autonomous mode.

1. model.py containing the script to create and train the model.
2. drive.py for driving the car in autonomous mode.
3. model.h5 containing a trained keras model.
4. video.mp4 a video recording of the ehicle driving autonomously around the track.

