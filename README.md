# Deep-Learning-Based-Annotation-Pipeline-for-Dashcam-Animal-Vehicle-Collision-Datasets
AI-assisted video annotation pipeline for dashcam-based animal–vehicle collision datasets using YOLO, ByteTrack, SAM, DeepSORT, and classical methods.


📌 Project Overview

This project focuses on developing an efficient, scalable, and AI-assisted annotation pipeline for dashcam footage captured in real-world road environments. The goal is to generate high-quality labels for training computer vision models that detect and analyze animal–vehicle collision (AVC) scenarios.

Traditional manual annotation is slow, inconsistent, and inefficient—especially for long video sequences. This project compares multiple annotation approaches and proposes hybrid methods combining tracking, segmentation, and human feedback to minimize annotation time while maintaining accuracy.

🚀 Key Features

Annotation of real dashcam footage captured in natural, uncontrolled environments

Multi-method comparison of annotation techniques:

YOLO + ByteTrack multi-object tracking

SAM segmentation (CVAT integrated)

DeepSORT tracking

SSD and RetinaNet detectors

Region Growing segmentation

Manual annotation using CVAT

Evaluation metrics include:

mAP, Precision, Recall, F1

MOTA, MOTP, ID switches (tracking)

IoU and Dice coefficient (segmentation)

Fully reproducible workflow including preprocessing, annotation, evaluation, and results

🧠 Annotation Methods Used
1️⃣ YOLO + ByteTrack (Tracking-Based)

Fast and highly accurate multi-object tracking

Maintains object IDs across frames

Significantly reduces manual labeling workload

Suitable for real-time applications

2️⃣ SAM (Segment Anything Model)

Provides pixel-level segmentation masks

Integrated into CVAT

Extremely accurate for object boundaries

Evaluated using IoU and Dice

3️⃣ DeepSORT

Uses deep appearance embeddings for stable tracking

Slightly more identity switches under complex scenes

4️⃣ SSD & RetinaNet

Single-shot detectors for frame-level object detection

RetinaNet handles rare/imbalanced classes better

5️⃣ Region Growing

Classical segmentation using seed expansion

Less robust under noisy lighting and motion

6️⃣ Manual CVAT Annotation

Ground-truth reference for all comparisons

📊 Evaluation Metrics
Detection Metrics

mAP (Mean Average Precision)

Precision

Recall

F1 Score

Tracking Metrics

MOTA

MOTP

ID Switches

Segmentation Metrics

IoU

Dice Score

🏆 Key Results

YOLO + ByteTrack achieved the highest performance in detection and tracking

SAM segmentation produced the most accurate pixel-level masks

Region Growing performed poorly under real road conditions

Manual annotation remains reliable but is the most time-consuming

This establishes modern AI-assisted annotation as the best approach for large-scale dashcam datasets.
