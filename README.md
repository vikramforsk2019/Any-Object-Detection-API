# Any-Object-Detection-API
by using this Flask api we can detect any object detection using yolo3.
we have only these 3 things requirement ---->

1.Pretrained weights file    (__name__.weights)
wget -P weights https://pjreddie.com/media/files/yolov3.weights

2.classes names file         (_name_.names)

3.yolov3_custum.cfg          (_name_.cfg)

in yolo_detection.py
---change to locations---->
#Give the configuration and weight files for the model and load the network using them.
  
   1.modelConfiguration = "yolov3_custom.cfg";
   2.modelWeights = "yolov3.weights";

# Load names of classes
   3.classesFile = "coco.names";

yolov3_custom.cfg

1.subdivisons=16/32
2.max_batches=(classes*2000) not less than 4000            (max_batches = 500200)

3.steps=80% of max_batches,90% of max_batches                  (ex.if steps=4000 then steps=3200,3600 if classes=1) (steps=400000,450000 if classes =80) or on 17 line
              
search yolo
4.filters=(classes+5)*3  filters (85*3)=255
classes=80


