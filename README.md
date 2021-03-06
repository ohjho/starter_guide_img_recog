# :rocket: A Starter Guide to Face Detection & Recognition in Python

[![made-with-python](https://img.shields.io/badge/Made%20with-Python-1f425f.svg)](https://www.python.org/)
[![MIT license](https://img.shields.io/badge/License-MIT-blue.svg)](https://lbesson.mit-license.org/)
![tested-on-osx](https://img.shields.io/badge/Tested%20on-OSX-lightgrey.svg)

## Table of Content
  * [Intro](#intro)
  * [How to Use this repo](#how-to-use-this-repo)
  * [Boilerplates](#clipboard-boilerplates)
  * [References](#references)
  * [Installing the Required Packages](#installing-the-required-packages)
  * [Credits](#pray-credits)
  * [License](#black_nib-license)

## Intro
To understand what is Facial Detection and/or recognition, you can read our [**primer**](_text_files/primer.md) or checkout a the [**slides**](https://gitpitch.com/ohjho/starter_guide_img_recog/master?p=_text_files) we made for our data science bootcamp presentation.

## How to Use this repo
1. Clone this repo:
```
$ git clone https://github.com/ohjho/starter_guide_img_recog.git
$ cd start_guide_img_recog
```
2. install the requirements. We **highly recommend** doing this inside a [virtualenv][url_virtualenv] and avoid [dependency hell](https://medium.com/knerd/the-nine-circles-of-python-dependency-hell-481d53e3e025).  
```
#---------------- optional ------------------
$ mkvirtualenv --python=`which python3` NameOfYourEnv
$ workon NameOfYourEnv
(NameOfYourEnv) $ pip freeze > uninstall.txt
(NameOfYourEnv) $ pip uninstall -r uninstall.txt -y
(NameOfYourEnv) $ rm uninstall.txt
#--------------------------------------------

(NameOfYourEnv) $ pip install -r requirements.txt
```
and just check and resolve any packages dependency issues if they show up under `pip check`. It should say `No broken requirements found.`  

You are not done yet :exclamation: If you are going to use the **dlib** or **yolo** templates in this guide, you will need to follow the [installation notes](#installing-the-required-packages).

3. Start Jupyter notebook
```
$ cd _templates
$ jupyter notebook
```
4. Have fun and go build some awesome projects! :surfer:

## :clipboard: Boilerplates
Want to start working on an Image Recognition project?!

Here are some **templates** to get yous started:
* ![badge testing](https://img.shields.io/badge/Status-Testing-Olive.svg)   [OpenCV](_templates/opencv_facedetection.ipynb)
* ![badge complete](https://img.shields.io/badge/Status-Completed-Green.svg)  [Dlib: HOG Face Detector](_templates/dlib_HOGfacedetector.ipynb)
* ![badge complete](https://img.shields.io/badge/Status-Completed-Green.svg)  [Dlib: Facial Landmarks Detector](_templates/dlib_faciallandmarksdetector.ipynb)
* ![badge work in progress](https://img.shields.io/badge/Status-Work%20In%20Progress-Orange.svg)  [YOLO2](_templates/yolo_v2.ipynb)

## References
### Tutorials
* [History of Facial Recongition](https://www.facefirst.com/blog/brief-history-of-face-recognition-software/)
* [Advancements in Facial Recognition Systems](https://medium.com/coinmonks/from-the-rand-tablet-to-differentiating-identical-twins-aa4ba6031bb0)
* An Intro [video by YoutTube star Siraj Raval](https://www.youtube.com/watch?v=4eIBisqx9_g&amp=&t=1116s)
* [Face Detection for Beginners](https://towardsdatascience.com/face-detection-for-beginners-e58e8f21aad9)
* [Face Recognition for Beginners](https://towardsdatascience.com/face-recognition-for-beginners-a7a9bd5eb5c2)
* [Methods for Face Detection and Face Recognition - A Review](https://medium.com/beesightsoft/methods-for-face-detection-and-face-recognition-a-review-57e73af1d67)
* [Modern Face Recognition with Deep Learning](https://medium.com/@ageitgey/machine-learning-is-fun-part-4-modern-face-recognition-with-deep-learning-c3cffc121d78)
* [Building a Face Detection Model from Video using Deep Learning](https://www.analyticsvidhya.com/blog/2018/12/introduction-face-detection-video-deep-learning-python/)
* [A Github Repo](https://github.com/llSourcell/YOLO_Object_Detection/blob/master/YOLO%20Object%20Detection.ipynb) on the recent development of face detection algorithm
#### Open CV
* [Face Recognition with Python, in Under 25 Lines of Code](https://realpython.com/face-recognition-with-python/)
* [Using OpenCV to play "Where's Waldo?"](https://machinelearningmastery.com/using-opencv-python-and-template-matching-to-play-wheres-waldo/)
* [OpenCV Face Recognition](https://www.pyimagesearch.com/2018/09/24/opencv-face-recognition/)
* [Facial Recognition in OpenCV, Python, and Deep Learning](https://www.pyimagesearch.com/2018/06/18/face-recognition-with-opencv-python-and-deep-learning/)
#### Dlib
* [HOG as object detector explained](http://blog.dlib.net/2014/02/dlib-186-released-make-your-own-object.html)
* [Make your own object detector with HOG](http://www.hackevolve.com/create-your-own-object-detector/)
* [Understanding dlib's facial landmark detector](https://www.pyimagesearch.com/2017/04/03/facial-landmarks-dlib-opencv-python/)
* [HOG vs CNN based face detector from dlib](https://towardsdatascience.com/cnn-based-face-detector-from-dlib-c3696195e01c)
* [Dlib's deep learning on facial recognition](http://blog.dlib.net/2017/02/high-quality-face-recognition-with-deep.html)
#### YOLO
* A [TED talk](https://www.youtube.com/watch?v=Cgxsv1riJhI) by one of the developer of YOLO
* A [video](https://www.youtube.com/watch?v=NM6lrxy0bxs) about how YOLO works
* [YOLO: Implementations and how to use them](https://medium.com/@monocasero/object-detection-with-yolo-implementations-and-how-to-use-them-5da928356035)
* [YOLOv2 object detection using Darkflow](https://towardsdatascience.com/yolov2-object-detection-using-darkflow-83db6aa5cf5f)
* [This repo](https://github.com/fountainhead-gq/YOLO_Collection) has implementation of YOLO in several flavours

### Libraries
* [OpenCV](https://opencv.org/)
* [dlib][url_dlib]
* [face_recognition][url_facerecog]
* [YOLOv2 using Darkflow][url_darkflow]

### Documentations
* [OpenCV-Python](https://opencv-python-tutroals.readthedocs.io/en/latest/py_tutorials/py_tutorials.html)
* [dlib](http://dlib.net/)
* The Darknet's guide to [YOLO](https://pjreddie.com/darknet/yolo/)

---

## Installing the Required Packages
### openCV
`requirements.txt` will install `opencv-contrib-python` for you. For more details, read this [installation guide](https://www.pyimagesearch.com/2018/09/19/pip-install-opencv/).
### face_detection/dlib
[`dlib`][url_dlib] is written in **C++**, so in order to use it we need to clone the [`dlib` repo][url_dlib] and compile it in python per this [instruction][url_dlib_installnote](make sure you satisfy the [pre-requisite](#dlib-pre-requisite) ). We **highly recommend** doing this inside a [**virtualenv**][url_virtualenv]:
```
$ cd to/your/git/dir
$ git clone https://github.com/davisking/dlib.git
$ cd dlib
$ mkdir build; cd build; cmake ..; cmake --build .
$ cd ..
$ python3 setup.py install
```
#### dlib Pre-requisite
* you need to have **Python3** installed. To check, type `which python3` in your command-line
* you need to have [**Homebrew**](https://brew.sh/). To install:
```
/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
```
* you need [X11](https://support.apple.com/en-hk/HT201341) to be installed **before** installing `dlib`, else you may experience [AttributeError](https://github.com/davisking/dlib/issues/302). To install: Head to [XQuartz](https://www.xquartz.org/) to download the latest version.
* you need to have `cmake`. To install: `brew install cmake`
### YOLO
There are currently three main implementations of YOLO:
1. **Darknet**: The 'offical' implementation written in C
2. **AlexeyAB/ Darknet**:  a fork of Darknet to support Windows and Linux
3. **Darkflow**: a port of Darknet over to TensorFlow.
   _Note_: the CPU-only Darkflow even runs faster than Darknet with the main drawback being the current Darkflow is not updated to YOLO3
#### Installing YOLOv2 (Darkflow)
In this guide, we will install the **Darkflow flavor of YOLOv2**. Again, we recommend the use of [**virtualenv**][url_virtualenv]:   
```
$ cd to/your/git/dir
$ git clone https://github.com/thtrieu/darkflow.git
$ cd darkflow
$ python setup.py build_ext --inplace
$ pip install .
```

[`pip install .`](https://askubuntu.com/questions/1067372/what-does-pip-install-dot-mean) basically install the package definitions from the current location i.e. darkflow.

##### Downloading Pre-trained Weights
Import the weights from [Darknet](https://pjreddie.com/darknet/yolo/) into the weights [_templates/weights](_templates/weights) directory.
```
wget https://pjreddie.com/media/files/yolov3.weights
mv yolov3.weights starter_guide_img_recog/_templates/weights/yolov3.weights
```

Alternatively, you can download the weights from the [Darkflow's author Google Drive](https://drive.google.com/drive/folders/0B1tW_VtY7onidEwyQ2FtQVplWEU) manually into [_templates/weights](_templates/weights).

---

## :pray: Credits
This project's main contributors are [@youonf](https://github.com/youonf) and [@agsl0905](https://github.com/agsl0905).

Special Thanks to [@samoshaughnessy](https://github.com/samoshaughnessy) for showing us how to use Git.  

## :black_nib: License
The content of this project is licensed under the [MIT license](_text_files/LICENSE)

[url_dlib]: https://github.com/davisking/dlib/
[url_dlib_installnote]: https://gist.github.com/ageitgey/629d75c1baac34dfa5ca2a1928a7aeaf
[url_facerecog]: https://github.com/ageitgey/face_recognition
[url_darkflow]: https://github.com/thtrieu/darkflow
[url_virtualenv]: https://virtualenvwrapper.readthedocs.io/en/latest/
