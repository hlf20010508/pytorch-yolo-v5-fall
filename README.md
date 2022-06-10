# pytorch-yolo-v5-fall

训练
```
python3 train.py --weights yolov5x.pt --epochs 50 --batch-size -1 --save-period 10
```
训练集配置保存在data/mydata.yaml
模型保存在runs/train/exp/weights/best.pt

测试
```
python3 detect.py --weights runs/train/exp/weights/best.pt --nosave --conf-thres 0 --iou-thres 0 --save-txt --source fall-test/test
```
--source为测试集路径，需要自行更改
