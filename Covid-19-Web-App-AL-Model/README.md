# COVID-19-Detection based on Chest X-rays and CT-Scans
COVID-19 Detection based on Chest X-rays and CT Scans using four Transfer Learning algorithms: VGG16, ResNet50, InceptionV3, Xception. The models were trained for 500 epochs on around 1000 Chest X-rays and around 750 CT Scan images on Google Colab GPU. After training, the accuracies acheived for the model are as follows:
<pre>
                InceptionV3  VGG16   ResNet50   Xception
Chest X-rays    96%          94%      83%       92%

CT Scans        93%          93%      80%       95%
</pre>
A Flask App was later developed wherein user can upload Chest X-rays or CT Scans and get the output of possibility of COVID infection.

# Dataset
The dataset for the project was gathered from two sources:

1. Chest X-ray images (1000 images) were obtained from: https://github.com/ieee8023/covid-chestxray-dataset

2. CT Scan images (750 images) were obtained from: https://github.com/UCSD-AI4H/COVID-CT/tree/master/Data-split

80% of the images were used for training the models and the remaining 20% for testing

# Evaluation and Results

<h3>Sample output of test images</h3><br>

<img src="https://github.com/kaushikjadhav01/COVID-19-Detection-Flask-App-based-on-Chest-X-rays-and-CT-Scans/blob/master/screenshots/sample_chest.PNG"> <img src="https://github.com/kaushikjadhav01/COVID-19-Detection-Flask-App-based-on-Chest-X-rays-and-CT-Scans/blob/master/screenshots/sample_ct.PNG">

<h3>Classification Reports for Chest X-rays:  VGG, InceptionV3, ResNet50, Xception </h3>

<img src="https://github.com/kaushikjadhav01/COVID-19-Detection-Flask-App-based-on-Chest-X-rays-and-CT-Scans/blob/master/flask%20app/assets/images/vgg_chest_report.PNG"> <img src="https://github.com/kaushikjadhav01/COVID-19-Detection-Flask-App-based-on-Chest-X-rays-and-CT-Scans/blob/master/flask%20app/assets/images/inception_chest_report.PNG">

<img src="https://github.com/kaushikjadhav01/COVID-19-Detection-Flask-App-based-on-Chest-X-rays-and-CT-Scans/blob/master/flask%20app/assets/images/resnet_chest_report.PNG"> <img src="https://github.com/kaushikjadhav01/COVID-19-Detection-Flask-App-based-on-Chest-X-rays-and-CT-Scans/blob/master/flask%20app/assets/images/xception_chest_report.PNG">

<h3>Confusion Matrix for Chest X-rays:  VGG, InceptionV3, ResNet50, Xception </h3>

<img src="https://github.com/kaushikjadhav01/COVID-19-Detection-Flask-App-based-on-Chest-X-rays-and-CT-Scans/blob/master/screenshots/vgg_chest_cm.PNG"> <img src="https://github.com/kaushikjadhav01/COVID-19-Detection-Flask-App-based-on-Chest-X-rays-and-CT-Scans/blob/master/screenshots/inception_chest_cm.PNG">

<img src="https://github.com/kaushikjadhav01/COVID-19-Detection-Flask-App-based-on-Chest-X-rays-and-CT-Scans/blob/master/screenshots/resnet_chest_cm.PNG"> <img src="https://github.com/kaushikjadhav01/COVID-19-Detection-Flask-App-based-on-Chest-X-rays-and-CT-Scans/blob/master/screenshots/xception_chest_cm.PNG">

<h3>Classification Reports for CT Scans:  VGG, InceptionV3, ResNet50, Xception </h3>

<img src="https://github.com/kaushikjadhav01/COVID-19-Detection-Flask-App-based-on-Chest-X-rays-and-CT-Scans/blob/master/flask%20app/assets/images/vgg_ct_report.PNG"> <img src="https://github.com/kaushikjadhav01/COVID-19-Detection-Flask-App-based-on-Chest-X-rays-and-CT-Scans/blob/master/flask%20app/assets/images/inception_ct_report.PNG">

<img src="https://github.com/kaushikjadhav01/COVID-19-Detection-Flask-App-based-on-Chest-X-rays-and-CT-Scans/blob/master/flask%20app/assets/images/resnet_ct_report.PNG"> <img src="https://github.com/kaushikjadhav01/COVID-19-Detection-Flask-App-based-on-Chest-X-rays-and-CT-Scans/blob/master/flask%20app/assets/images/xception_ct_report.PNG">

<h3>Confusion Matrix for CT Scans:  VGG, InceptionV3, ResNet50, Xception </h3>

<img src="https://github.com/kaushikjadhav01/COVID-19-Detection-Flask-App-based-on-Chest-X-rays-and-CT-Scans/blob/master/screenshots/vgg_ct_cm.PNG"> <img src="https://github.com/kaushikjadhav01/COVID-19-Detection-Flask-App-based-on-Chest-X-rays-and-CT-Scans/blob/master/screenshots/inception_ct_cm.PNG">

<img src="https://github.com/kaushikjadhav01/COVID-19-Detection-Flask-App-based-on-Chest-X-rays-and-CT-Scans/blob/master/screenshots/resnet_ct_cm.PNG"> <img src="https://github.com/kaushikjadhav01/COVID-19-Detection-Flask-App-based-on-Chest-X-rays-and-CT-Scans/blob/master/screenshots/xception_ct_cm.PNG">

<h3>Screenshots of Flask App</h3>

<img src="https://github.com/kaushikjadhav01/COVID-19-Detection-Flask-App-based-on-Chest-X-rays-and-CT-Scans/blob/master/screenshots/banner.PNG">

<img src="https://github.com/kaushikjadhav01/COVID-19-Detection-Flask-App-based-on-Chest-X-rays-and-CT-Scans/blob/master/screenshots/banner2.PNG" width="150%">

# Technical Concepts
<b>ImageNet</b> is formally a project aimed at (manually) labeling and categorizing images into almost 22,000 separate object categories for the purpose of computer vision research.<br>
More information can be found <a href="https://www.pyimagesearch.com/2017/03/20/imagenet-vggnet-resnet-inception-xception-keras/">here</a>
<br>
<br>
<b>ResNet50</b> ResNet-50 is a convolutional neural network that is 50 layers deep. You can load a pretrained version of the network trained on more than a million images from the ImageNet database. The pretrained network can classify images into 1000 object categories, such as keyboard, mouse, pencil, and many animals. Unlike traditional sequential network architectures such as AlexNet, OverFeat, and VGG, ResNet is instead a form of “exotic architecture” that relies on micro-architecture modules.<br>
More information can be found <a href="https://www.mathworks.com/help/deeplearning/ref/resnet50.html#:~:text=ResNet%2D50%20is%20a%20convolutional,%2C%20pencil%2C%20and%20many%20animals.">here</a>
<br>
<br>
<b>VGG16</b> is a convolutional neural network model proposed by K. Simonyan and A. Zisserman from the University of Oxford in the paper “Very Deep Convolutional Networks for Large-Scale Image Recognition”. The model achieves 92.7% top-5 test accuracy in ImageNet, which is a dataset of over 14 million images belonging to 1000 classes. <br>
More information can be found <a href="https://www.mathworks.com/help/deeplearning/ref/resnet50.html#:~:text=ResNet%2D50%20is%20a%20convolutional,%2C%20pencil%2C%20and%20many%20animals.">here</a>
<br>
<br>
<b>Inception-V3</b> is a convolutional neural network that is 48 layers deep. You can load a pretrained version of the network trained on more than a million images from the ImageNet database. The pretrained network can classify images into 1000 object categories, such as keyboard, mouse, pencil, and many animals. As a result, the network has learned rich feature representations for a wide range of images. The network has an image input size of 299-by-299.<br>
More information can be found <a href="https://www.mathworks.com/help/deeplearning/ref/resnet50.html#:~:text=ResNet%2D50%20is%20a%20convolutional,%2C%20pencil%2C%20and%20many%20animals.">here</a>
<br>
<br>
<b>Xception</b> is a convolutional neural network that is 71 layers deep. You can load a pretrained version of the network trained on more than a million images from the ImageNet database. The pretrained network can classify images into 1000 object categories, such as keyboard, mouse, pencil, and many animals. As a result, the network has learned rich feature representations for a wide range of images. The network has an image input size of 299-by-299. <br>
More information can be found <a href="https://www.mathworks.com/help/deeplearning/ref/resnet50.html#:~:text=ResNet%2D50%20is%20a%20convolutional,%2C%20pencil%2C%20and%20many%20animals.">here</a>


## How to use Flask App
<ul>
  <li>Download repo, change to directory of repo, go to command prompt and run <b>pip install -r requirements.txt</b></li>
  <li>On command prompt, run <b>python app.py</b></li>
  <li>Open your web browser and go to <b>127.0.0.1:5000</b> to access the Flask App</li>
</ul>
