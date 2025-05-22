# 🛰️ Space Station Object Detection — Duality AI Hackathon

This repository contains our solution for the **Duality AI - Space Station Hackathon**. We trained a YOLOv8 model using synthetic data from Duality AI’s Falcon platform to detect three critical objects in a simulated space station environment:

- 🔧 Toolbox  
- 🧯 Fire Extinguisher  
- 🛢️ Oxygen Tank  

---

## 📁 Project Structure

📦 Aithon-Team-Vision.AI-main/
├── train.py # Script to train YOLOv8 model
├── predict.py # Script for inference and evaluation
├── config.yaml # YOLOv8-compatible config file
├── runs/ # Folder containing training logs and PR/F1 curves
├── weights/
│ └── best.pt # Final trained YOLOv8 weights
├── data/
│ ├── train/, val/, test/ # Falcon synthetic dataset (YOLO format)
├── Report.pdf # Final 8-page performance report
├── Use_Case.pdf # (Optional) Bonus application description
├── README.md # You are here


---

## 🚀 How to Run the Project

### 🔧 1. Set Up Environment

Make sure you have [Anaconda](https://www.anaconda.com/products/distribution) installed.

``` bash ```
conda create -n EDU python=3.9 -y
conda activate EDU
pip install ultralytics opencv-python matplotlib torch torchvision torchaudio

📈 3. Run Inference & Evaluate
bash
Copy
Edit
python predict.py
Generates:

mAP@0.5 and mAP@0.5:0.95

Precision-Recall curves

F1-Confidence curve

Sample predictions

Confusion Matrix (optional)



# 🧠 Model Highlights
Metric	Value
mAP@0.5	0.941
Precision	0.99
Recall	0.91
Best F1 Score	0.94

✅ Fire Extinguisher: 0.962

✅ ToolBox: 0.936

✅ Oxygen Tank: 0.925


