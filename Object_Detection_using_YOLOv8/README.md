<img src="README Img/header.png" alt="Header"/>

<h1 align="center">Object Detection using YOLOv8</h1>

## 🚀 About YOLO:

One type of computer vision task is object detection, which involves locating a certain object in images or videos. This is a very important task which has applications in numerous tasks like robotics, self driving cars,  and surveillance. One of the earliest methods used for this task was sliding window technique, R-CNN. YOLO is one such deep learning technique which uses a single-shot to detect object in images. The full form of it is you only look once. It detects objects in single pass and therefore is very useful in real time object detection tasks.YOLO (You Only Look Once) uses an end-to end neural network that makes prediction of object class and the object boundary at once. There are several versions of YOLO with v9 being the latest one. More information on it is available at [https://arxiv.org/abs/1506.02640](https://arxiv.org/abs/1506.02640).

## 💭Project Process:

The images data which contains images is downloaded from [Open Image Dataset V7](https://storage.googleapis.com/openimages/web/index.html) with the annotations required to train. The YOLOv8 nano model is trained using the images and annotations.  The train set used is 800 images and test set is 200 images. The model is tested using the images from the test set. The plotted graphs show that the loss decreases over the 20 epochs. 

Check [Google Colab](https://github.com/AdityaMN98/Projects/tree/main/Object_Detection_using_YOLOv8/Google_Collab) directory for the code.

## 🛠️Steps:
- Get the images which have the object which has to be detected.
- Check for annotations or annotate the images using tools like cvat.ai.
- Store the images and labels in the YOLO format.
- Create the yaml file having the path to images both training and evaluation set with the classes in the images.
- Use the appropriate YOLOv8 Model. Train and test the model using the data. Refer [Ultralytics YOLO](https://github.com/ultralytics/ultralytics) for the models and training process.

## 📊Results:

The graphs produced after training are shown below.

<img src="README Img/results.png" alt="results" height = 300 width = 1000/>

The trained model is used to detect the object(car).

<img src="README Img/img1.jpg" alt="img1" height = 150 width = 270/> <img src="README Img/img1_out.jpg" alt="img1out" height = 150 width = 270/>

The model does not detect all the cars in below image. To improve a larger model with more parameters can be used with more images and annotations to train the model.

<img src="README Img/img2.jpg" alt="img1" height = 150 width = 270/> <img src="README Img/img2_out.jpg" alt="img1out" height = 150 width = 270/>


## ⚡Technologies and Applications Used:

- `Python`
- `Ultralytics YOLOv8`
- `Annotations - cvat.ai`
- `Convoluted Neural Networks`
- `Open Image Dataset V7 - Data`

## 📈Improvements:

- Can use small, medium, large YOLOv8 model.
- Use data augmentation for better results on unseen images. 
- Using more images to train the model, can give better object detection.
- Can get better results by using above techniques when more than one object is in image like image 2 in results.