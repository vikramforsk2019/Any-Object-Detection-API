# Any-Object-Detection-API
Creating Flask api and object detection using yolo3.
we have only these 3 things requirements:

# 1.Pretrained weights file    (yolov3.weights)
https://pjreddie.com/media/files/yolov3.weights
<br>
copy it,in yolo_files/ 
# 2.classes names file         (coco.names)
present in repo not require
# 3.yolov3_custum.cfg          (yolov3_custom.cfg)
present in repo
# requirements
pip install requirement.txt
# Run the app.py
python app.py <br>
localhost:5000/

# Example Input
![babu](https://user-images.githubusercontent.com/51817568/87654983-4458e900-c775-11ea-8c07-fa5cdf94235a.png)
# OUTPUT
![babu_yolo_out_py](https://user-images.githubusercontent.com/51817568/87655737-3fe10000-c776-11ea-8fb2-3f3c0e35a99d.jpg)

# how can update yolov3_custom.cfg(Not Require for this repo project already done)
# 1.subdivisons=16/32
<br>
if classes=80 <br>
# 2.max_batches=(classes*2000)
 (min_batches=4000,max_batches = 500200) <br>
Note: if classes=1 then max_batches=4000 
<br>
# 3.steps=80% of max_batches,90% of max_batches <br>
(ex. steps=3200,3600 if classes=1)      <br> 
(steps=400000,450000 if classes =80) <br> 
( on 17 line) <br>
4.filters=(classes+5)*3   
<br>
filters= (80+5)*3=255 
# last give classes name in coco.names
then finish updating.ok


