<h1 align="center">Face Mask Detection Program</h1>






  







 

 
## Project Demo
[Demo Link](https://www.youtube.com/watch?v=m-MlgJ-__y8)







## Tech/framework used

- [OpenCV](https://opencv.org/)
- [Keras](https://keras.io/)
- [TensorFlow](https://www.tensorflow.org/)
- [MobileNetV2](https://arxiv.org/abs/1801.04381)

## Features
The face mask detector didn't use any morphed masked images dataset. The model is accurate, and since we used the MobileNetV2 architecture, it’s also computationally efficient and thus making it easier to deploy the model to embedded systems (Raspberry Pi, Google Coral, etc.).

This system can therefore be used in real-time applications which require face-mask detection for safety purposes due to the outbreak of Covid-19. This project can be integrated with embedded systems for application in airports, railway stations, offices, schools, and public places to ensure that public safety guidelines are followed.


This dataset consists of __3835 images__ belonging to two classes:
*	__with_mask: 1916 images__
*	__without_mask: 1919 images__
The dataset is propriotery. Please email me at ghosh_deb@hotmail.com to gain access to it.

## Prerequisites

All the dependencies and required libraries are included in the file <code>requirements.txt</code>
## How to run
1. Clone the repo
```
$ git clone https://github.com/chandrikadeb7/Face-Mask-Detection.git
```

2. Change your directory to the cloned repo and create a Python virtual environment named 'test'
```
$ conda create -n ml-fmd pip python==3.7
```

3. Now, run the following command in your Terminal/Command Prompt to install the libraries required
```
$ pip3 install -r requirements.txt
```

4. Open terminal. Go into the cloned project directory folder and type the following command:
```
$ python train_mask_detector.py --dataset dataset
```

5. To detect face masks in real-time video streams type the following command:
```
$ python3 detect_mask_video.py 
```
## Results

![](https://github.com/chandrikadeb7/Face-Mask-Detection/blob/master/Readme_images/Screenshot%202020-06-01%20at%209.48.27%20PM.png)

![](https://github.com/chandrikadeb7/Face-Mask-Detection/blob/master/Readme_images/Screenshot%202020-06-01%20at%209.48.27%20PM.png)

#### The model gave 98% accuracy for Face Mask Detection after training via <code>tensorflow-gpu==2.0.0</code>

![](https://github.com/chandrikadeb7/Face-Mask-Detection/blob/master/Readme_images/Screenshot%202020-06-01%20at%209.48.27%20PM.png)

ps: use only tensorflow==2.0.0 if you do not have a dedicated GPU

#### I got the following accuracy/loss training curve plot
![](https://github.com/chandrikadeb7/Face-Mask-Detection/blob/master/plot.png)







## Owner
Made by [Debankur Ghosh](https://github.com/Debankur-C137)

## License
MIT © 
