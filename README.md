# Raccoon Detector Dataset

<img src="raccoon-demo.gif" alt="Overview" width="60%" height="60%">

This repo are based on [this blog post](https://medium.com/towards-data-science/how-to-train-your-own-object-detector-with-tensorflows-object-detector-api-bec72ecfe1d9) This is a dataset that collected to train my own Raccoon detector with [TensorFlow's Object Detection API](https://github.com/tensorflow/models/tree/master/research/object_detection). Images are from Google and Pixabay. In total, there are 200 images (180 are used for training and 20 for validation).

## Getting Started

##### Folder Structure:
```
+ bbox_label: contains the hand labeled xml files in PASCAL VOC format
+ data: contains the input file for the TF object detection, the pipeline configuration file, frozen model and labelmap.
+ images: contains the image data in jpg format
- a few handy scripts: xml_to_tfrecord.py is used to generate the input files directly from bbox_label/*.xml files to tf recordfor the TF API. train.py is copied from TensorFlow's Object Detection API where the training is happening. export_terminal.txt is the sample that could run in terminal


```

