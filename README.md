

![alt text](videos/project_video_augmented.gif "Result")



## Project Overview

In order to detect the lane lines in a video stream we must accomplish the folowing:
Camera Calibration
Color Transform
Perspective Transform
Lane Pixel Detection
Image augmentation
Pipeline

## Reflection
1. Identify potential shortcomings with your current pipeline
![alt text](videos/challenge_video_augmented.gif "Result")
We can clearly see that the pipeline start to struggle, this is because this video adds features like a concrete seperator that projects a shadow into the lane and paralel to the lane lines. Close to the camera the model works relatively well but near the escape point we can see the lane detection starting to fail.
![alt text](videos/harder_challenge_video_augmented.gif "Result")
It's obvious that the model does not perform well. The lane boundary is "all over the place" and could not keep the car inside the lane. This is most likely due to the nature of the road, single line for each traffic direction, steeper bends and a higher proximity to the side of the road.