# Any-Object-Detection-API
by using this Flask api we can detect any object detection using yolo3.
we have only these 3 things requirement ---->

1.Pretrained weights file    (__name__.weights)

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

  
-- LICENSE
|-- OID
|   |-- Dataset
|   |   |-- train
|   |   |   `-- Aircraft_Weapon
|   |   |       |-- 000731dd242627f2.jpg
|   |   |       |-- 000731dd242627f2.txt
|   |   |       |-- 0007ff438786b5ff.jpg
|   |   |       |-- 0007ff438786b5ff.txt
|   |   |       |-- 000b9a97776b3634.txt
|   |   |       |-- 00117a00b1dc48dc.jpg
|   |   |       |-- 00117a00b1dc48dc.txt
|   |   |       |-- 0012619786e2ef90.jpg
|   |   |       |-- 0012619786e2ef90.txt
|   |   |       |-- 0013356a9d5d526a.jpg
|   |   |       |-- 0013356a9d5d526a.txt
|   |   |       |-- 00144844bdaf8351.jpg
|   |   |       |-- 00144844bdaf8351.txt
|   |   |       |-- 0017e63e7bb111f8.jpg
|   |   |       |-- 0017e63e7bb111f8.txt
|   |   |       |-- 001edeee73440b15.jpg
|   |   |       |-- 001edeee73440b15.txt
|   |   |       |-- 001eec76ef36e679.jpg
|   |   |       |-- 001eec76ef36e679.txt
|   |   |       |-- 002172c48265b973.jpg
|   |   |       |-- 002172c48265b973.txt
|   |   |       |-- 0021ea873f2e416e.jpg
|   |   |       |-- 0021ea873f2e416e.txt
|   |   |       |-- 0023b0e23b369b8d.jpg
|   |   |       |-- 0023b0e23b369b8d.txt
|   |   |       |-- 002f9eba0ed54904.jpg
|   |   |       |-- 002f9eba0ed54904.txt
|   |   |       |-- 002ff6e1eecb80b8.jpg
|   |   |       |-- 002ff6e1eecb80b8.txt
|   |   |       |-- 003883a134d9869e.jpg
|   |   |       |-- 003883a134d9869e.txt
|   |   |       |-- 003b2d3c807da35f.jpg
|   |   |       |-- 003b2d3c807da35f.txt
|   |   |       |-- 00410cf982be7b7c.jpg
|   |   |       |-- 00410cf982be7b7c.txt
|   |   |       |-- 00414f0e16bafe10.jpg
|   |   |       |-- 00414f0e16bafe10.txt
|   |   |       |-- 00559e8576ad8108.jpg
|   |   |       |-- 00559e8576ad8108.txt
|   |   |       |-- 0056595e121189ca.jpg
|   |   |       |-- 0056595e121189ca.txt
|   |   |       |-- 0057f6a4bf6997a9.jpg
|   |   |       |-- 0057f6a4bf6997a9.txt
|   |   |       |-- 005b47528e6a32cb.jpg
|   |   |       |-- 005b47528e6a32cb.txt
|   |   |       `-- Label
|   |   |           |-- 000731dd242627f2.txt
|   |   |           |-- 0007ff438786b5ff.txt
|   |   |           |-- 000b9a97776b3634.txt
|   |   |           |-- 00117a00b1dc48dc.txt
|   |   |           |-- 0012619786e2ef90.txt
|   |   |           |-- 0013356a9d5d526a.txt
|   |   |           |-- 00144844bdaf8351.txt
|   |   |           |-- 0017e63e7bb111f8.txt
|   |   |           |-- 001edeee73440b15.txt
|   |   |           |-- 001eec76ef36e679.txt
|   |   |           |-- 002172c48265b973.txt
|   |   |           |-- 0021ea873f2e416e.txt
|   |   |           |-- 0023b0e23b369b8d.txt
|   |   |           |-- 002f9eba0ed54904.txt
|   |   |           |-- 002ff6e1eecb80b8.txt
|   |   |           |-- 003883a134d9869e.txt
|   |   |           |-- 003b2d3c807da35f.txt
|   |   |           |-- 00410cf982be7b7c.txt
|   |   |           |-- 00414f0e16bafe10.txt
|   |   |           |-- 00559e8576ad8108.txt
|   |   |           |-- 0056595e121189ca.txt
|   |   |           |-- 0057f6a4bf6997a9.txt
|   |   |           `-- 005b47528e6a32cb.txt
|   |   `-- validation
|   |       `-- Apple_Orange
|   |           |-- 0471d3e80e3b5a37.jpg
|   |           |-- 078821d86db99fc9.jpg
|   |           |-- 08cd15d3912ca157.jpg
|   |           |-- 09a06df60e4bdd62.jpg
|   |           |-- 0b6f22bf3b586889.jpg
|   |           |-- 0baea327f06f8afb.jpg
|   |           |-- 0d6db81d71062441.jpg
|   |           |-- 0fdea8a716155a8e.jpg
|   |           |-- 105433f9d808d18e.jpg
|   |           |-- 183d9d5fd2379cf9.jpg
|   |           |-- 195157a8957c2b89.jpg
|   |           |-- 1e6efc60e52f7919.jpg
|   |           |-- 1ec9c56575adf1c5.jpg
|   |           |-- 1fc8f9c0630fa13d.jpg
|   |           |-- 22cf78f0eb8e7f25.jpg
|   |           |-- 26e9c1d28f09f186.jpg
|   |           |-- 275f429194a6683a.jpg
|   |           |-- 2fe4f21e409f0a56.jpg
|   |           |-- 32bd80d38fc5b085.jpg
|   |           |-- 34ab650dd6093346.jpg
|   |           |-- 37a867029f2e7868.jpg
|   |           |-- 3b3a23644d0ba4b1.jpg
|   |           |-- 3c9c2fa9dcb03246.jpg
|   |           |-- 3e810338e95a9cee.jpg
|   |           |-- 3eabeff9361b226f.jpg
|   |           |-- 4163d30eba358af1.jpg
|   |           |-- 41e2356b97f775c4.jpg
|   |           |-- 43af5611777d4f1c.jpg
|   |           |-- 4e67aea79a236b7d.jpg
|   |           |-- 500d6cdc7e8fb3e1.jpg
|   |           |-- 500ef7bbed25b42d.jpg
|   |           |-- 52c33abf081b58ce.jpg
|   |           |-- 5384a150e18efbb5.jpg
|   |           |-- 53912158f0b7dfce.jpg
|   |           |-- 53b4f49b09747d35.jpg
|   |           |-- 55985cfdc2aff31b.jpg
|   |           |-- 562ed1cbbcd50f38.jpg
|   |           |-- 598ab2035a9a7f53.jpg
|   |           |-- 5b78c9ffb1961209.jpg
|   |           |-- 5d89f7273f94eb32.jpg
|   |           |-- 65c2280668db3f33.jpg
|   |           |-- 672649d03eb7248b.jpg
|   |           |-- 69974d01b659acfe.jpg
|   |           |-- 69f3f3889793e68e.jpg
|   |           |-- 6e9f89a2758892d3.jpg
|   |           |-- 6f5f56c01df801c7.jpg
|   |           |-- 7000732d55384f88.jpg
|   |           |-- 79f629405dd16464.jpg
|   |           |-- 7e6a885c298febf5.jpg
|   |           |-- 80448eba6de10241.jpg
|   |           |-- 8120a85e31ebaea4.jpg
|   |           |-- 89f81119b54c2448.jpg
|   |           |-- 8c3a108e102e3414.jpg
|   |           |-- 8c5c8e7a603fac3e.jpg
|   |           |-- 8c7d69610416a787.jpg
|   |           |-- 8ce6d8afb2779d20.jpg
|   |           |-- 94de58da0f25a821.jpg
|   |           |-- 9afb8f2d68b727d3.jpg
|   |           |-- 9d00f2d303c4ec5d.jpg
|   |           |-- 9e1a8092c3c7fce7.jpg
|   |           |-- Label
|   |           |   |-- 0471d3e80e3b5a37.txt
|   |           |   |-- 078821d86db99fc9.txt
|   |           |   |-- 08cd15d3912ca157.txt
|   |           |   |-- 09a06df60e4bdd62.txt
|   |           |   |-- 0b6f22bf3b586889.txt
|   |           |   |-- 0baea327f06f8afb.txt
|   |           |   |-- 0d6db81d71062441.txt
|   |           |   |-- 0fdea8a716155a8e.txt
|   |           |   |-- 105433f9d808d18e.txt
|   |           |   |-- 183d9d5fd2379cf9.txt
|   |           |   |-- 195157a8957c2b89.txt
|   |           |   |-- 1e6efc60e52f7919.txt
|   |           |   |-- 1ec9c56575adf1c5.txt
|   |           |   |-- 1fc8f9c0630fa13d.txt
|   |           |   |-- 22cf78f0eb8e7f25.txt
|   |           |   |-- 26e9c1d28f09f186.txt
|   |           |   |-- 275f429194a6683a.txt
|   |           |   |-- 2fe4f21e409f0a56.txt
|   |           |   |-- 32bd80d38fc5b085.txt
|   |           |   |-- 34ab650dd6093346.txt
|   |           |   |-- 37a867029f2e7868.txt
|   |           |   |-- 3b3a23644d0ba4b1.txt
|   |           |   |-- 3c9c2fa9dcb03246.txt
|   |           |   |-- 3e810338e95a9cee.txt
|   |           |   |-- 3eabeff9361b226f.txt
|   |           |   |-- 4163d30eba358af1.txt
|   |           |   |-- 41e2356b97f775c4.txt
|   |           |   |-- 43af5611777d4f1c.txt
|   |           |   |-- 4e67aea79a236b7d.txt
|   |           |   |-- 500d6cdc7e8fb3e1.txt
|   |           |   |-- 500ef7bbed25b42d.txt
|   |           |   |-- 52c33abf081b58ce.txt
|   |           |   |-- 5384a150e18efbb5.txt
|   |           |   |-- 53912158f0b7dfce.txt
|   |           |   |-- 53b4f49b09747d35.txt
|   |           |   |-- 55985cfdc2aff31b.txt
|   |           |   |-- 562ed1cbbcd50f38.txt
|   |           |   |-- 598ab2035a9a7f53.txt
|   |           |   |-- 5b78c9ffb1961209.txt
|   |           |   |-- 5d89f7273f94eb32.txt
|   |           |   |-- 65c2280668db3f33.txt
|   |           |   |-- 672649d03eb7248b.txt
|   |           |   |-- 69974d01b659acfe.txt
|   |           |   |-- 69f3f3889793e68e.txt
|   |           |   |-- 6e9f89a2758892d3.txt
|   |           |   |-- 6f5f56c01df801c7.txt
|   |           |   |-- 7000732d55384f88.txt
|   |           |   |-- 79f629405dd16464.txt
|   |           |   |-- 7e6a885c298febf5.txt
|   |           |   |-- 80448eba6de10241.txt
|   |           |   |-- 8120a85e31ebaea4.txt
|   |           |   |-- 89f81119b54c2448.txt
|   |           |   |-- 8c3a108e102e3414.txt
|   |           |   |-- 8c5c8e7a603fac3e.txt
|   |           |   |-- 8c7d69610416a787.txt
|   |           |   |-- 8ce6d8afb2779d20.txt
|   |           |   |-- 94de58da0f25a821.txt
|   |           |   |-- 9afb8f2d68b727d3.txt
|   |           |   |-- 9d00f2d303c4ec5d.txt
|   |           |   |-- 9e1a8092c3c7fce7.txt
|   |           |   |-- a0c7bb3a01ecc4b9.txt
|   |           |   |-- a18f3669c64970b1.txt
|   |           |   |-- a34275c238d98efa.txt
|   |           |   |-- a4dd75d633c1d657.txt
|   |           |   |-- a6fa6e875d6ae7fd.txt
|   |           |   |-- a70275d426badec1.txt
|   |           |   |-- a9eaae4555ad0a96.txt
|   |           |   |-- aa41598448363fd5.txt
|   |           |   |-- ac4836e92d94b93f.txt
|   |           |   |-- b2d9f62471971548.txt
|   |           |   |-- b4cb895b4eb903a4.txt
|   |           |   |-- b5c57763b0dad42c.txt
|   |           |   |-- b6fb83d9e81594cd.txt
|   |           |   |-- b87bb9d6db36a333.txt
|   |           |   |-- b88d7ed92b910aca.txt
|   |           |   |-- becc028793504bdc.txt
|   |           |   |-- c0a32ea06e59d966.txt
|   |           |   |-- c2c19be58ed7280b.txt
|   |           |   |-- c552e01cc9f3f0be.txt
|   |           |   |-- c76492c4b4a52985.txt
|   |           |   |-- c78165afc346ece0.txt
|   |           |   |-- c82701a86cd96018.txt
|   |           |   |-- c90f57a9d8fceb90.txt
|   |           |   |-- c99db9c3802cb506.txt
|   |           |   |-- c9b24d97c7649819.txt
|   |           |   |-- c9ebd63bc789073a.txt
|   |           |   |-- cb5edca45155e5ba.txt
|   |           |   |-- d0ac2231cb048520.txt
|   |           |   |-- d1fd3e3f620c0af5.txt
|   |           |   |-- d208ab3ec41b37ce.txt
|   |           |   |-- db1af159a2c0fef4.txt
|   |           |   |-- dbdae6a1b9f5e18b.txt
|   |           |   |-- deef6ea77bdb97e9.txt
|   |           |   |-- dfec55965c1cdf19.txt
|   |           |   |-- e1d5de98ce2559e7.txt
|   |           |   |-- e2903d7029b5067d.txt
|   |           |   |-- e2e7cae075ad9aa2.txt
|   |           |   |-- e417ab70bcfa87b0.txt
|   |           |   |-- ed37c41b16636962.txt
|   |           |   |-- ed8c8cbff74c7ad1.txt
|   |           |   |-- f04b1b8d0d4abb46.txt
|   |           |   |-- f168f75ef492fc4d.txt
|   |           |   |-- f6d564bd1a412584.txt
|   |           |   |-- f7e81cf48de05419.txt
|   |           |   |-- f9705847c26e33b3.txt
|   |           |   |-- fc8cd78dcd066490.txt
|   |           |   `-- ff3e3f98de225575.txt
|   |           |-- a0c7bb3a01ecc4b9.jpg
|   |           |-- a18f3669c64970b1.jpg
|   |           |-- a34275c238d98efa.jpg
|   |           |-- a4dd75d633c1d657.jpg
|   |           |-- a6fa6e875d6ae7fd.jpg
|   |           |-- a70275d426badec1.jpg
|   |           |-- a9eaae4555ad0a96.jpg
|   |           |-- aa41598448363fd5.jpg
|   |           |-- ac4836e92d94b93f.jpg
|   |           |-- b2d9f62471971548.jpg
|   |           |-- b4cb895b4eb903a4.jpg
|   |           |-- b5c57763b0dad42c.jpg
|   |           |-- b6fb83d9e81594cd.jpg
|   |           |-- b87bb9d6db36a333.jpg
|   |           |-- b88d7ed92b910aca.jpg
|   |           |-- becc028793504bdc.jpg
|   |           |-- c0a32ea06e59d966.jpg
|   |           |-- c2c19be58ed7280b.jpg
|   |           |-- c552e01cc9f3f0be.jpg
|   |           |-- c76492c4b4a52985.jpg
|   |           |-- c78165afc346ece0.jpg
|   |           |-- c82701a86cd96018.jpg
|   |           |-- c90f57a9d8fceb90.jpg
|   |           |-- c99db9c3802cb506.jpg
|   |           |-- c9b24d97c7649819.jpg
|   |           |-- c9ebd63bc789073a.jpg
|   |           |-- cb5edca45155e5ba.jpg
|   |           |-- d0ac2231cb048520.jpg
|   |           |-- d1fd3e3f620c0af5.jpg
|   |           |-- d208ab3ec41b37ce.jpg
|   |           |-- db1af159a2c0fef4.jpg
|   |           |-- dbdae6a1b9f5e18b.jpg
|   |           |-- deef6ea77bdb97e9.jpg
|   |           |-- dfec55965c1cdf19.jpg
|   |           |-- e1d5de98ce2559e7.jpg
|   |           |-- e2903d7029b5067d.jpg
|   |           |-- e2e7cae075ad9aa2.jpg
|   |           |-- e417ab70bcfa87b0.jpg
|   |           |-- ed37c41b16636962.jpg
|   |           |-- ed8c8cbff74c7ad1.jpg
|   |           |-- f04b1b8d0d4abb46.jpg
|   |           |-- f168f75ef492fc4d.jpg
|   |           |-- f6d564bd1a412584.jpg
|   |           |-- f7e81cf48de05419.jpg
|   |           |-- f9705847c26e33b3.jpg
|   |           |-- fc8cd78dcd066490.jpg
|   |           `-- ff3e3f98de225575.jpg
|   `-- csv_folder
|       |-- class-descriptions-boxable.csv
|       |-- train-annotations-bbox.csv
|       `-- validation-annotations-bbox.csv
|-- README.md
|-- classes.txt
|-- convert_annotations.py
|-- images
|   |-- classes.png
|   |-- rectangle.png
|   `-- visualizer_example.gif
|-- main.py
|-- modules
|   |-- __pycache__
|   |   |-- bounding_boxes.cpython-37.pyc
|   |   |-- csv_downloader.cpython-37.pyc
|   |   |-- downloader.cpython-37.pyc
|   |   |-- image_level.cpython-37.pyc
|   |   |-- parser.cpython-37.pyc
|   |   |-- show.cpython-37.pyc
|   |   `-- utils.cpython-37.pyc
|   |-- bounding_boxes.py
|   |-- csv_downloader.py
|   |-- downloader.py
|   |-- image_level.py
|   |-- parser.py
|   |-- show.py
|   `-- utils.py
`-- requirements.txt
