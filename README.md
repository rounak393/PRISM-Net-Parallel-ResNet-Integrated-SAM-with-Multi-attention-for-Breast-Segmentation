# 🌟 PRISM-Net: Parallel ResNet-Integrated-SAM with Multi-attention

PRISM-Net is a specialized, vision-forward deep learning architecture engineered for precision breast ultrasound lesion segmentation. By running a foundational zero-shot model (FastSAM) in parallel with a robust convolutional backbone (ResNet-50), it captures both sweeping semantic context and granular anatomical nuances. Enhanced by edge-aware operators and a multi-attention fusion mechanism, PRISM-Net homes in on critical tumor boundaries while actively silencing background acoustic noise.

---

## 🏛️ The Architecture

> <img width="960" height="540" alt="Architecures" src="https://github.com/user-attachments/assets/b46b4639-0fb9-4e31-9f24-33cf1abed117" />


---

## 🏆 Performance Benchmarks

Precision is everything in medical imaging. Here is how PRISM-Net holds up against standard benchmark datasets:

| Dataset | Dice Coefficient (DSC) | Intersection over Union (IoU) |
| :--- | :---: | :---: |
| **BUSI** | `[ 85.10 ]` | `[ 74.06 ]` |
| **BUSBRA** | `[ 91.31 ]` | `[ 84.27 ]` |


## 🔬 Error Analysis

To build trust in medical AI, we need to know exactly where the model struggles. Our error mapping visualizes the network's decision boundaries directly against the ground truth.

> **[🖼️ UPLOAD ERROR ANALYSIS IMAGE HERE]**  
<img width="971" height="315" alt="BUSIERROR" src="https://github.com/user-attachments/assets/0b58364e-b681-4655-b6f2-28e68afdbe54" />
BUSI ERROR ANALYSIS
<img width="950" height="315" alt="BUSERROR" src="https://github.com/user-attachments/assets/6542b6ad-a5ea-48c1-a9d2-eb9bddeb4585" />


* ⬜ **Pure White:** True Positives *(Spot-on tissue identification)*
* 🟥 ** Red:** False Positives *(Background hallucinated as a tumor / Over-segmentation)*
* 🟦 ** Blue:** False Negatives *(Missed tumor regions / Under-segmentation)*

---

## 🧠 Model Interpretability (Grad-CAM)

We don't just want a black box. Using Gradient-weighted Class Activation Mapping (Grad-CAM), we peek into the network's "mind" to ensure it is focusing on true pathological features rather than irrelevant image artifacts.

><img width="950" height="315" alt="BUSIGRADCAM" src="https://github.com/user-attachments/assets/732b7f34-e8a3-41cd-8e8e-aa457ef4ceca" />
<img width="950" height="315" alt="BUSGRADCAM" src="https://github.com/user-attachments/assets/8ab2f58a-59c2-40d7-b8fd-5030f5525df5" />




---

## ✍️ Authors

* **Rounak Saha** 
* **Dr.Britika Khati**
* **Dr.Ram Sarkar**
