# YOLO11 Object Detection Training Project
## Professional Technical Portfolio

---

## 1. Project Objective
This project implements end-to-end object detection model training and evaluation using the **YOLO11n** lightweight deep learning model. The core objectives are:
- Train a high-performance object detector on the COCO128 benchmark dataset
- Analyze model convergence, loss trends, and detection metrics
- Build a standardized, reproducible AI training workflow for technical documentation
- Demonstrate practical deep learning engineering skills

## 2. Model & Environment
- **Model**: YOLO11n (Nano, lightweight real-time object detector)
- **Framework**: PyTorch + Ultralytics
- **Hardware**: MacBook Air M1 (CPU training)
- **Dataset**: COCO128 (128 images, 80 object categories)
- **Python Version**: 3.10.20

## 3. Training Configuration
```bash

# Full training command
yolo detect train model=yolo11n.pt data=coco128.yaml epochs=50 imgsz=640 batch=2



Epochs: 50
Image size: 640×640
Batch size: 2
Optimizer: Auto (AdamW)
Loss functions: box_loss, cls_loss, dfl_loss

##4. Usage Instructions
Training
Run the command above to start training from scratch.
Evaluation
The model automatically validates after each epoch and saves the best weights.
Inference
Use the trained best.pt for object detection on new images/videos.

##5. Key Findings & Performance Metrics
After 50 training epochs, the model achieved strong performance:
Precision: 0.788
Recall: 0.690
mAP@0.5: 0.762
mAP@0.5:0.95: 0.578

## Training Observations
Loss values decreased steadily, indicating stable model convergence
No obvious overfitting during the entire training process
The lightweight YOLO11n model balances speed and accuracy effectively
High-performance categories: person, airplane, motorcycle, stop sign

## Conclusion
This project successfully completes the full pipeline of object detection model training, including environment setup, data configuration, model training, performance evaluation, and result visualization. The trained YOLO11n model delivers reliable detection performance, and this repository serves as a standardized technical portfolio for deep learning engineering practices. 
