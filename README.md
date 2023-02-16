# Celestial scanner
Celestial Scanner is a satellite simulator made with Tensorflow and the Object Detection API, able to detect space celestial objects like asteroids, planets, galaxies, nebulas and black holes.

### Model
To create the model i first gathered image data of all the selestial objects i needed to detect, (asteroids, planets, galaxies, nebulas and black holes). I then labeled each object using the LabelImg tool and split them into test and training. Afterwards i created the label map of my classes and generated the tfrecords of my dataset, test and train accordingly. Next step was to get a pre-trained model from tensorflow model zoo and in my case i used the SSD MobileNet V2 FPNLite 320x320 model. Final step was to tweak the appropriate fields of the models pipeline file for my data directories and trained the model with 2000 steps and saved it, after running few tests i took the ready model and used it on this final repository.

## Requirements
To use the model you are going to need:
- Tensorflow
- OpenCV
- Matplotlib
- Object-Detection

** To install Tensorflow Object Detection API you need to follow the installation steps from [here](https://github.com/tensorflow/models/blob/master/research/object_detection/g3doc/tf2.md)

## Pictures
![test1](https://user-images.githubusercontent.com/75722160/218894043-71213c9f-001c-4679-b0de-4481c85799e3.png)
![test2](https://user-images.githubusercontent.com/75722160/218894058-22bd7c12-6f55-4d4e-959d-28c680c426aa.png)
![test3](https://user-images.githubusercontent.com/75722160/218894063-df00f83b-0804-43dc-9fb8-5bbdfb22fe50.png)
