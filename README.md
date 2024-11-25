# Overwatch 2 Players Detector

#### Supported Labels
['Head']

#### Model:
- YOLO11l: https://huggingface.co/jparedesDS/ow2-yolo11m

#### ALL my models YOLO11, YOLOv10 & YOLOv9
- YOLO11l: https://huggingface.co/jparedesDS/fluorescent-penetrant-inspection
- YOLO11x: https://huggingface.co/jparedesDS/welding-defects-detection
- YOLOv9c: https://huggingface.co/jparedesDS/cs2-yolov9c
- YOLOv10s: https://huggingface.co/jparedesDS/cs2-yolov10s
- YOLOv10m: https://huggingface.co/jparedesDS/cs2-yolov10m
- YOLOv10b: https://huggingface.co/jparedesDS/cs2-yolov10b
- YOLOv10b: https://huggingface.co/jparedesDS/valorant-yolov10b
- YOLO11m: https://huggingface.co/jparedesDS/valorant-yolo11m
- YOLO11l: https://huggingface.co/jparedesDS/deadlock-yolo11l

#### How to use
```
from ultralytics import YOLO

# Load a pretrained YOLO model
model = YOLO(r'weights\ow2-yolo11m.pt')

# Run inference on 'image.png' with arguments
model.predict(
    'image.png',
    save=True,
    device=0
    )
```
#### Confusion matrix normalized
![confusion_matrix_normalized.png](https://cdn-uploads.huggingface.co/production/uploads/62e1c9b42e4cab6e39dafc97/qZnMSqcob_Fn9KesMNi3V.png)
#### Labels
![labels.jpg](https://cdn-uploads.huggingface.co/production/uploads/62e1c9b42e4cab6e39dafc97/m6jFSPdcmfBON21EbnKzH.jpeg)
#### Results
![results.png](https://cdn-uploads.huggingface.co/production/uploads/62e1c9b42e4cab6e39dafc97/GqivS6eBWLGn2h-rIQOql.png)
#### Predict
![val_batch1_labels.jpg](https://cdn-uploads.huggingface.co/production/uploads/62e1c9b42e4cab6e39dafc97/gVSp_0IK1HeNqt8HwXwKQ.jpeg)
![val_batch2_labels.jpg](https://cdn-uploads.huggingface.co/production/uploads/62e1c9b42e4cab6e39dafc97/dPS8W2IRXSwZCrj0L_1gk.jpeg)
```
YOLO11m summary (fused): 303 layers, 20,030,803 parameters, 0 gradients, 67.6 GFLOPs
                 Class     Images  Instances      Box(P          R      mAP50  mAP50-95): 100%|██████████| 4/4 [00:01<00:00,  2.69it/s]
                   all        273        133      0.742      0.563       0.66      0.317
```

#### Others models...
https://huggingface.co/jparedesDS/
