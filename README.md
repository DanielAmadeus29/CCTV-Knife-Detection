# CCTV-Knife-Detection
This project focuses on **knife detection in CCTV / surveillance-style footage** using a YOLO-based object detection model.  
The goal is to improve detection performance in real-world public video sources where knives may appear small, blurred, partially occluded, or affected by low-quality recording conditions.

Google Colab:  
[Open Notebook](https://colab.research.google.com/drive/1QENTmuOk2ZAcSLCBFH9njeXqYoMOXUIo?usp=sharing)
## Dataset

The dataset used in this project is a **combined dataset from Simuletic and Roboflow** to increase data variety and better reflect different surveillance-style scenarios.
- **Simuletic Dataset:** [CCTV Knife Detection Dataset](https://simuletic.com/datasets)
- **Roboflow:** [Roboflow Universe](https://universe.roboflow.com/mbb-hrfxf/knife-detection-3wp7q)

**Total dataset size:** **2,192 images**

### Data Split
- **Train:** 1,569 images
- **Validation:** 415 images
- **Test:** 208 images

## Model Performance

Best result achieved at **epoch 20**:

- **mAP50:** 0.9592
- **mAP50-95:** 0.6355
- **Precision:** 0.9512
- **Recall:** 0.9019

Test videos were evaluated using **raw public-source videos** collected from platforms such as:
- Twitter / X
- Reddit
- Other public online sources

Test Result Folder:  
[View Test Results](https://drive.google.com/drive/folders/1jEE8RKCaa0GLQS86eDcsVrGpjN4i9Kh5?usp=sharing)

## Notes

Since this project targets **surveillance camera scenarios**, performance on real-world footage can still be challenging due to:
- low resolution
- motion blur
- occlusion
- poor lighting
- small knife objects in frame
- domain differences between training images and public CCTV footage

