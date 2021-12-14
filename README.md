# helmet-project
Auto helmet detection using computer vision algorithm

Project for bachelor thesis

The project source code files are organized as below:
- `construction-image-detecion-final.ipynb`: Loads data from Google Drive to Colab environment, Preprocesses data and Trains model with yolov5 package. You should run this ipython notebook at Colab and your drive should contain folder `Helmet-Project` which contains ACID_6000.zip and Human-Body.zip
- `detect.py`: YOLOv5 package's object detecting module which is an [open source](https://github.com/ultralytics/yolov5). If you want to try object detection form Youtube video, type `python detect.py --weights runs/train/yolo5s_construction_human/weights/best.pt --source 'https://youtu.be/MHaZXSneOGQ'`

The project source data files are organized as below:
- `ACID_6000`: Contains 6,000 images of construction machines with annotation directories. The data is received from AIRCon-Lab, so you should contact Xiao, B (bxiao2@ualberta.ca) to get data
- `Human-Body`: Contains human gesture image with annotations. Label boxes' location and size is contained in `MPHB-label-txt/MPHB-label.txt`. You can download data from [Multiple Pose Human Body Database](http://parnec.nuaa.edu.cn/_upload/tpl/02/db/731/template731/pages/xtan/MPHB.html)

Run the ipynb file at Colab with data ready at Google Drive. Then you download the trained weights to `yolov5/` directory and run `detect.py` module.

Youtube links used for detection:
1. [Biggest Rc Construction-Site in the World! Rc Truck Action at Minibaustelle Alsfeld 2017!
](https://youtu.be/MHaZXSneOGQ)
2. [Amazing Dangerous Fastest Excavator Operator Skill, Heavy Equipment Machines Truck Working Fail]
(https://youtu.be/ZgbXp4HmAdY)
