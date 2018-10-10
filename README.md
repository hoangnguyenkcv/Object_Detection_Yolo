# Object_Detection_Yolo
1. Enviroment: 
+ keras: 2.2.2
+ tensorflow: 1.10
+ python: 2.5

2. Initialization preparation 
+ download COCO 2014 dataset from http://cocodataset.org/#download
extract file train2014.zip to forder .\\COCO_dataset\\images\\train2014
extract file val2014.zip to forder .\\COCO_dataset\\images\\val2014
extract file annotations_trainval2014.zip to forder .\\COCO_dataset\\annotations

+ to convert annotations in COCO format to VOC format, create forder .\\VOC\\train and .\\VOC\\val, then run: 

python coco2pascal.py create_annotations COCO_dataset/annotations train VOC/train
python coco2pascal.py create_annotations COCO_dataset/annotations val VOC/val

+ Download pre-trained weights from https://pjreddie.com/darknet/yolo/
        + https://pjreddie.com/media/files/yolo.weights

3. Training and validation 
+ run file yolo_object_detection.ipynb

