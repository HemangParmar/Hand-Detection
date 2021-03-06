<!-- PROJECT LOGO -->
<br />
<p align="center">
  <h3 align="center">Hand Detection</h3>

  <p align="center">
    Hand segmentation using Skin color and Motion Detection
    <br />
  </p>
</p>

<!-- TABLE OF CONTENTS -->
<details open="open">
  <summary>Table of Contents</summary>
  <ol>
    <li>
      <a href="#about-the-project">About The Project</a>
      <ul>
        <li><a href="#built-with">Built With</a></li>
      </ul>
    </li>
    <li>
      <a href="#getting-started">Getting Started</a>
      <ul>
        <li><a href="#installation">Installation</a></li>
      </ul>
    </li>
    <li><a href="#usage">Usage</a></li>
    <li><a href="#results">Results</a></li>
    <li><a href="#contact">Contact</a></li>
  </ol>
</details>

<!-- ABOUT THE PROJECT -->
## About The Project

Human-Computer Interaction using hand gesture recognition is a great advancement in technology that makes our life easier and convenient. For any gesture recognition, Hand detection is important that is a pre-processing step. In this project, hand segmentation is done using skin color and motion detection using thresholding. Using a web camera, the hand is segmented and then we can use it in any application. 

Hand segmentation using two methods: 1) Skin color detection 2) Motion detection using thresholding

### Built With

* [Python](https://www.python.org/)
* [Opencv](https://opencv.org/)

<!-- GETTING STARTED -->
## Getting Started

To get started, first need to install all important libraries for image processing. 

### Hardware

A simple web cam or any other external camera. 

### Installation

List of things you need to install.
* pip

  ```sh
  pip install opencv-python 
  ```
  ```sh
  pip install imutils
  ```
  ```sh
  pip install numpy
  ```
## Libraries

Opencv - Opencv is a library for computer vision, machine learning and image processing.

## Some functionality
### Apply threshold value to the image

Befor applying it, convert image into grayscale
```sh
thresh = cv.threshold(imgray, 127, 255, 0)
```
### Find and draw contours

```sh
contours, hierarchy = cv.findContours(thresh, cv.RETR_TREE, cv.CHAIN_APPROX_SIMPLE)
```

```sh
cv.drawContours(img, contours, -1, (0,255,0), 3)
```

###

<!-- USAGE EXAMPLES -->
## Usage

Hand gesture recognition using in many areas for human-computer interaction. HCI can makes our life easier and faster. Hand gesture is the best way to interact with the machines. To control the robot, sign language recognition, etc are the example of its applications.

## Results

#### Hand Detection using Skin color:

Combination of HSV and YCbCr model is used for hand segmentation. 

![Original](https://user-images.githubusercontent.com/77574279/129291577-cc314ea2-12ba-4bde-96b3-85eef7a1b4a3.jpg)

#### Hue, Saturation and Value color model

![HSV](https://user-images.githubusercontent.com/77574279/129238612-b716ac3b-d889-46cd-8473-36d1e5a389ca.jpg)

#### YCbCr (Luminance and Chrominance color model)
![YCbCr_](https://user-images.githubusercontent.com/77574279/129238674-44d13cb4-9dcc-4287-a3bb-aff4585116b7.jpg)

#### Result - Combination of HSV and YCbCr color model
![Final](https://user-images.githubusercontent.com/77574279/129238720-0c24c948-7b43-4e14-82d4-b8fb3443ab95.jpg)


### Hand detection using motion detection using thresholding:

Otsu's method selects the threshold value automatically and assigned to the image. Then Contours are drawn around the hand region to extract the hand. 

![FinalHand](https://user-images.githubusercontent.com/77574279/129291504-b88ea04b-41dc-4f17-99b8-dd5d7bf3ad0a.jpeg)


<!-- CONTACT -->
## Contact

Your Name - Hemang Parmar - hparmar6@lakeheadu.ca.com

Project Link: [https://github.com/HemangParmar/Hand-Detection](https://github.com/HemangParmar/Hand-Detection)

Project Presentation Link : [Youtube](https://youtu.be/2rlejWirJXg)


## References

https://docs.opencv.org/4.5.2/d6/d00/tutorial_py_root.html

[https://github.com/CHEREF-Mehdi/SkinDetection]

[https://github.com/dtaneja123/Hand_Recognition/blob/master/Hand_gesture_final.py]
