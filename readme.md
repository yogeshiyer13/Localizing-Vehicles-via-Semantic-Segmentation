### Introduction

This is a project in which we use the Deep Seeded Region Growing [DSRG](https://github.com/speedinghzl/DSRG) and implemet it using tensorflow. The DSRG is referring to the approach for weakly-supervised semantic segmentation in the paper ["Weakly-Supervised Semantic Segmentation Network with Deep Seeded Region Growing"](https://github.com/speedinghzl/DSRG). 

### About 

Semantic segmentation, is a novel image annotating approach, coming towards “Classification” and “Object Detection”. As we know, classification is the process of determining the type of object to which the input image belongs to, also called as “image-level label”; and “Object Detection” a process providing information about the location and size of the image. Semantic Segmentation deals with labelling individual pixels of the images as an instance of object classes.

For the scope of this project, we consider a semantic segmentation algorithm on the urban scenes, to investigate its performance on one of its most crucial applications, autonomous driving. Recent developments in image processing, especially object detection, put the researchers in this field towards inventing reliable smart self-driving cars. Since such cars are going to be designed for moving around streets, alleys, highways, and other parts of cities and megacities, it is vital for the groups working on implementing these smart vehicles to provide their autonomous cars with strong understanding of the urban scenes like traffic lights, road signs, pedestrians, and different types of vehicles; because even one false prediction from the side of the automotive cars might cause irrecoverable financial and health consequences

The Deep Seeded Region Growing (DSRG), is a deep neural network whose objective is to be trained for reaching initial cues of the image-level labelled data, and expand them in the order that the whole image is classified in either an object group or background.


### Preparation

for using this code, you have to do something else:

##### 1. Install pydensecrf

For using the densecrf in python, we turn to the project [pydensecrf](https://github.com/lucasb-eyer/pydensecrf). And you just using the following code to install it.

> pip install pydensecrf

##### 2. Download the data and model

1. for MIOTCD data set, please refer to its [official website](http://podoce.dinf.usherbrooke.ca/challenge/dataset/). For this project we are using a subset of MIOTCD dataset.
2. for localization_cues-cal.pickle, please referring to [DSRG](https://github.com/speedinghzl/DSRG) or [BaiduNetdisk](https://pan.baidu.com/s/14a94qw4nBulqqKHLMbQGUg)(which fetching code is qgig). And download it and extract it in the data/.
3. for init.model, you can download it from [googledriver](https://drive.google.com/file/d/1kxDguwRaIDm5WS6JTNzi8GO-HqKJqKnm/view) or [BaiduNetdisk](https://pan.baidu.com/s/1Q1wmAX7Do9jvvLMt3_8tFw). Just download it and put it in model/.

### Training

Then, you just input the following sentence to train it.

> python DSRG.py <gpu_id>
### Methodology 
The DSRG method looks something like this!
![DSRG Methodology](DSRG.JPG)    

### Result

Our results looked like this!

![Results](Result.JPG)

### Trained model
The trained model can be seen from here!
[google_driver](https://drive.google.com/open?id=1hlSl1EaDKWA00hvd6Ar0xDZ9uOZ7HKYu)
[BaiduNetdisk](https://pan.baidu.com/s/1vITyeBR5kxaGcOF0BHGkJA)

