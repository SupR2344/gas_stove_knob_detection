# Gas Stove Knob Detection

A YOLOv9s-based object detection project for detecting gas stove knobs and identifying their operating state as **ON** or **OFF**.

## Overview

This project uses the YOLOv9s object detection model trained on a custom gas stove dataset.

The model detects gas stove knobs and classifies each detected knob into one of two classes:

- `knob_OFF` — Gas stove knob is OFF
- `knob_ON` — Gas stove knob is ON

The trained model is provided as `best.pt`.

## Model

- Model: YOLOv9s
- Task: Object Detection
- Number of Classes: 2
- Input Image Size: 800 × 800
- Training Epochs: 150
- Batch Size: 32

## Classes

| ID | Class |
|---|---|
| 0 | knob_OFF |
| 1 | knob_ON |

## Dataset

The dataset is divided into three subsets:

```text
gas_stove_dataset/
├── train/
│   ├── images/
│   └── labels/
│
├── valid/
│   ├── images/
│   └── labels/
│
├── test/
│   ├── images/
│   └── labels/
│
└── data.yaml