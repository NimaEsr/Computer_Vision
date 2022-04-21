# Transfer learning with MobileNetV2

MobileNetV2 was trained on ImageNet and is optimized to run on mobile and other low-power applications. It's 155 layers deep  and very efficient for object detection and image segmentation tasks, as well as classification tasks like this one. The architecture has three defining characteristics:

*   Depthwise separable convolutions
*   Thin input and output bottlenecks between layers
*   Shortcut connections between bottleneck layers

<img src="MobilenetV2.png" style="width:300px;height:220px;">

MobileNetV2 uses depthwise separable convolutions as efficient building blocks. Traditional convolutions are often very resource-intensive, and  depthwise separable convolutions are able to reduce the number of trainable parameters and operations and also speed up convolutions. We will use MobileNetV2 that was designed to provide fast and computationally efficient performance. It's been pre-trained on ImageNet, a dataset containing over 14 million images and 1000 classes.

In this project, we aim to do transfer learning on a pre-trained CNN to build an Alpaca/Not Alpaca classifier!

<img src="alpaca.avif" style="width:300px;height:220px;">

We use a pretrained model to modify the classifier task so that it's able to recognize alpacas in three steps:

* Delete the top layer (the classification layer)

* Add a new classifier layer

* Freeze the base model and train the newly-created classifier layer
