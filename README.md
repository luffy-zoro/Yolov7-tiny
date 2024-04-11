# Yolov7-tiny
# training
Single GPU training
python train.py --workers 8 --device 0 --batch-size 32 --data data/kitti.yaml --img 640 640 --cfg cfg/training/yolov7.yaml --weights '' --name yolov7-tiny --hyp data/hyp.scratch.tiny.yaml
