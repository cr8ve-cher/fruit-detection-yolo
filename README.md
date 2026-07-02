# Fruit Detection using YOLO11

This project explores computer vision using a custom-trained YOLO11 model to detect fruits in images.
The goal was to understand the end-to-end object detection pipeline, from dataset creation to model training and inference.

## Dataset
- Custom dataset consisting of three classes: Apple, Banana, and Grapes
- Images sourced from a larger dataset and manually curated
- Bounding boxes annotated using Roboflow
- Exported in YOLO format with a data.yaml configuration file

Link to Dataset on Roboflow
https://tinyurl.com/mfnxc5p8

## Model and Training
- Model: YOLO11s
- Optimizer: AdamW
- Learning rate and early stopping were tuned for stability
- Data augmentation applied (HSV, scale, translation, mosaic)
- Trained for up to 80 epochs on Google Colab GPU

Link to Google Collab
https://tinyurl.com/ynba6nxx

## Results
Training artifacts are stored in the train/ directory:
- best.pt: best-performing trained weights
- results.png: visualization of loss and mAP metrics
- args.yaml: training configuration
<img width="2400" height="1200" alt="results" src="https://github.com/user-attachments/assets/69918506-6e29-4704-89db-ef01dbf77c26" />

## Inference and Export
The trained model was exported and tested locally using VS Code.
Inference was performed on custom images to validate real-world performance.

## Tools Used
- Ultralytics YOLO
- PyTorch
- Google Colab (GPU)
- Roboflow
