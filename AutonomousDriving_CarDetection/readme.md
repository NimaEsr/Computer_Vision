
In this project, we work on a self-driving car. As a critical component of this project, we would like to first build a car detection system. To collect data, we use a mounted camera to the hood (meaning the front) of the car, which takes pictures of the road ahead every few seconds as you drive around. 

</center>
<img src="test.png" style="width:450px;height:320px;">
</center>

Dataset provided by <a href="https://www.drive.ai/">drive.ai</a>.

We will use YOLO ("You Only Look Once") object detection algorithm, and apply it to car detection. Many of the ideas in this notebook are described in the two YOLO papers: [Redmon et al., 2016](https://arxiv.org/abs/1506.02640) and [Redmon and Farhadi, 2016](https://arxiv.org/abs/1612.08242). 
