# Yolov7-tiny
Object detection model based on improved YOLOv7-tiny
# Performance
On the KITTI dataset, the parameter number and computation amount of the improved YOLOv7-tiny algorithm decrease by 35.7% and 34.1% respectively, and the accuracy of the improved YOLOv7-TINY algorithm only decreases slightly. mAP@0.5 decreases by 1.7%, mAP@0.5:0.95 decreases by 0.6%, and tiny-object mAPs decreases by 1.2%. The improved algorithm model is tiny in size and is suitable for deployment on edge devices.
# training
Single GPU training
python train.py --workers 8 --device 0 --batch-size 32 --data data/kitti.yaml --img 640 640 --cfg cfg/training/yolov7.yaml --weights '' --name yolov7-tiny --hyp data/hyp.scratch.tiny.yaml
