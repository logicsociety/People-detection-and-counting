# **👥 People Detection & Counting System — Team Tracka Nova**

## **Index**

1. [Project Overview](#project-overview)
2. [Team Members](#team-members)
3. [Event & Timeline](#event--timeline)
4. [Problem Statement](#problem-statement)
5. [Technical Approach](#technical-approach)
6. [Dataset Details](#dataset-details)
7. [Model Training Pipeline](#model-training-pipeline)
8. [Output & Results](#output--results)
9. [Features](#features)
10. [How to Run the Project](#how-to-run-the-project)
11. [Requirements](#requirements)
12. [Future Enhancements](#future-enhancements)
13. [Applications](#applications)
14. [Acknowledgements](#acknowledgements)

---

## **Project Overview**

This project focuses on building a **People Detection and Counting System** using **YOLOv8**, trained on a custom dataset.
Instead of developing a completely new model, the objective was to understand **how a real object detection pipeline works**, from dataset preparation to training and prediction.

The system:

* Detects humans in images
* Draws bounding boxes
* Counts the number of people
* Works on image-based inputs using a pre-trained + fine-tuned YOLOv8 model



---

## **Team Members**

**Team Name — *Tracka Nova***

* **Karan Dalal (Mentor)**
* **Namaswi Tiwari (Team Leader)**
* **Pragya Goyal**
* **Palak Mundhara**
* **Ashwika Kashyap**

---

## **Event & Timeline**

This project was created as part of the **Avinay 2025** AI/ML initiative under Logic Society.

---

## **Problem Statement**

Crowd monitoring remains one of the most critical needs in:

* Public events
* Malls & metro stations
* Campus surveillance
* Smart city applications

Traditional systems require manual effort or expensive hardware.
This project explores a **cost-effective AI-based pipeline** for detecting and counting people using deep learning.

---

## **Technical Approach**

The project uses:

* **Roboflow** for dataset preparation and annotation
* **YOLOv8s** for training a lightweight people detection model
* **Google Colab** for running the training pipeline
* **Ultralytics** for both training and inference
* **Python + OpenCV** for visualization

All key training and inference logic is included in the `.py` and `.ipynb` files:


---

## **Dataset Details**

* **500 annotated images** downloaded & formatted using **Roboflow**
* Includes diverse human poses and crowd scenarios
* Exported in YOLOv8 format
* Basic augmentations applied before training


---

## **Model Training Pipeline**

As seen in project files:

1. Install YOLOv8 & Roboflow
2. Import dataset from Roboflow
3. Load the YOLOv8s pretrained model
4. Train the model for **25 epochs**, with:

   * Image size: **500×500**
   * Resumable training enabled
5. Run inference on uploaded sample images

Training script and prediction steps are available in:

* `people_detection_and_counting.py`


---

## **Output & Results**

* Bounding boxes drawn around detected people
* Count of total persons displayed
* Output displayed using YOLO’s `.show()` method
* Accuracy was limited due to:

  * Small dataset size
  * Hardware constraints
  * Low training epochs

Still, the project successfully demonstrated:

* Dataset → Model → Detection pipeline
* Hands-on understanding of practical deep learning workflows


---

## **Features**

* ✔️ People detection using YOLOv8
* ✔️ Bounding box visualisation
* ✔️ Automated people count
* ✔️ Custom dataset training
* ✔️ Lightweight, fast model
* ✔️ Beginner-friendly, extendable pipeline

---

## **How to Run the Project**

### **1. Clone the Repository**

```
git clone <your-repo-link>
cd people-detection-counting
```

### **2. Install Dependencies**

```
pip install ultralytics roboflow opencv-python pillow numpy
```

### **3. Run Inference**

Place your test image (e.g., `test.jpg`) in the project folder.

```
python people_detection_and_counting.py
```

### **4. (Optional) Re-train the Model**

Open the Colab notebook `.ipynb` file uploaded in the repository and run all cells.

---

## **Requirements**

* Python 3.8+
* YOLOv8 / Ultralytics
* Roboflow SDK
* OpenCV
* NumPy, PIL

---

## **Future Enhancements**

* Integration with **live CCTV feeds**
* Real-time dashboard for people flow monitoring
* Expand dataset to improve accuracy
* Deployment on **Raspberry Pi / Jetson Nano**
* Use DeepSORT / ByteTrack for people tracking



---

## **Applications**

* 🚇 Metro station monitoring
* 🎫 Event crowd management
* 🏫 School/college campus tracking
* 🏢 Workplace attendance analysis
* 🚶 Smart city population analytics

---

## **Acknowledgements**

This project was created under **Logic Society** during **Avinay 2025**.
Special thanks to:

* **Roboflow** for dataset creation tools
* **Ultralytics** for YOLOv8
* **Google Colab** for training environment
