# Any-Object-Detection-API
by using this Flask api we can detect any object detection using yolo3.
we have only these 3 things requirement ---->

# 1.Pretrained weights file    (__name__.weights)
wget -P weights https://pjreddie.com/media/files/yolov3.weights
copy in yolo_files/ folder
# 2.classes names file         (coco.names.names)
present in repo
# 3.yolov3_custum.cfg          (yolov3_custom.cfg)
present in repo
# requirements
pip install requirement,txt
# Run the app.py
python app.py <br>
localhost:5000/
# yolo_detection.py
1.modelConfiguration = "yolov3_custom.cfg";
2.modelWeights = "yolov3.weights";
3.classesFile = "coco.names";

# how can update yolov3_custom.cfg(Not Require for this repo project)
1.subdivisons=16/32

2.max_batches=(classes*2000) not less than 4000            (max_batches = 500200)

3.steps=80% of max_batches,90% of max_batches (ex.if steps=4000 then steps=3200,3600 if classes=1) (steps=400000,450000 if classes =80) or on 17 line search yolo
4.filters=(classes+5)*3  filters (85*3)=255
classes=80
# Example Input
![babu](https://user-images.githubusercontent.com/51817568/87654983-4458e900-c775-11ea-8c07-fa5cdf94235a.png)
# OUTPUT
![babu_yolo_out_py](https://user-images.githubusercontent.com/51817568/87654975-41f68f00-c775-11ea-9249-eb168bf20f33.jpg)

