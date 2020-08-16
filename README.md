# Autonomous Self-driving Car in GTA-5 #
## Demo ##
### Driving on the Highway ###
![gif](Demo/demo1.gif)
### Driving in the City ###
![gif](Demo/demo2.gif)

Note: AI is trained on the highway, but still performs relative well in the city.
## About ##
The goal of this project is to build a self-driving car with deep learning and computer vision, which can navigate in different environments. The project is inspired by the work done by Sentdex. After experimenting with different convolutional neural networks, NVIDIA's PilotNet is choosen for faster prediction rate. YOLOv3, one of the most popular object detection alogorithm, is also integrated with PilotNet to add steering, throttle and brake control as per traffic density.
## Setup and Requirements ##
1. Grand Theft Auto-5 (turn on hood camera)
2. Pyhton 3.6
3. Tensorflow
4. Keras
5. OpenCV
6. Numpy
7. Pygame
8. Xbox 360 Emulator(https://www.x360ce.com/)
9. vJoy (http://vjoystick.sourceforge.net/site/)
## Dataset ##
### My Dataset ###
100,000 images with respective steering angle and throttle is collected by driving the car on the highway. However, only 39,046 images are left after balancing the data, therefore the dataset is arficially expanded by fliping the image along the horizontal axis, and multiplying the steering angle by -1. 

Dataset used to trained this model can be found here: https://drive.google.com/drive/folders/1R787vkWaMe5nsWyLpbXTG55aUv4YteTo?usp=sharing
### Custom Dataset ###
Using collect_data.py to generate your custom dataset. Ensure the GTA-5 window size same as in the collect_data.py
Upload the collected data on Google Drive to train your model on Google Colab. 
## Training (Google Colab) ##
Training code can be found here: https://colab.research.google.com/drive/1hjLdVByL0oQxfrcpVlDJgqU9cvNahyaW?usp=sharing
## Usage ## 
## Future Improvements ##
## Acknowledgement ##
