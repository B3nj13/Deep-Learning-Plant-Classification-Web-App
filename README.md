# Multiple object detection using Transfer Learning on MobilenetV3 in TensorFlow.js

## What can it do?

Using a machine learning model to recognize multiple objects on image to be presented to it. Even better, not only is it found that the image contains an object, but it can also get the co-ordinates of the bounding box for each object it finds, which allows highlighting of the found object in the image. 

Loading a model using the ImageNet-SSD architecture, to [recognize 90 common objects](https://github.com/tensorflow/tfjs-models/blob/master/coco-ssd/src/classes.ts) the model has already been taught to find from the [COCO dataset](http://cocodataset.org/#home).


## In the files:

### ← index.html

Script tags in our HTML to grab the latest version of TensorFlow.js and the machine learning model class that can take image data as input and output predictions for what it sees in that image data.

reference the following to bring in TensorFlow.js:

```HTML
<script src="https://cdn.jsdelivr.net/npm/@tensorflow/tfjs/dist/tf.min.js" type="text/javascript"></script>
```
```
pull in the machine learning model class we later use in script.js like this:

```HTML
<script src="https://cdn.jsdelivr.net/npm/@tensorflow-models/coco-ssd"></script>
```

### ← style.css

 styles to make the prototype look prettier.

### ← script.js

Code written in JavaScript to interact with the COCO-SSD class imported in the HTML. Passes the data to the class and then retrives predictions on what it thinks it saw in the image which can be used to make a decision. 

---
