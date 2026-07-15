# 🌟 PRISM-Net: Parallel ResNet-Integrated-SAM with Multi-attention

PRISM-Net is a specialized, vision-forward deep learning architecture engineered for precision breast ultrasound lesion segmentation. By running a foundational zero-shot model (FastSAM) in parallel with a robust convolutional backbone (ResNet-50), it captures both sweeping semantic context and granular anatomical nuances. Enhanced by edge-aware operators and a multi-attention fusion mechanism, PRISM-Net homes in on critical tumor boundaries while actively silencing background acoustic noise.

---

## 🏛️ The Architecture

> **[🖼️ UPLOAD ARCHITECTURE IMAGE HERE]**
> <img width="960" height="540" alt="Architecures" src="https://github.com/user-attachments/assets/b46b4639-0fb9-4e31-9f24-33cf1abed117" />

> *(Drag and drop your architecture diagram into the GitHub editor right here, then replace the dummy link below with the generated one!)*

![PRISM-Net Architecture Blueprint](link_to_architecture_image.png)

---

## 🏆 Performance Benchmarks

Precision is everything in medical imaging. Here is how PRISM-Net holds up against standard benchmark datasets:

| Dataset | Dice Coefficient (DSC) | Intersection over Union (IoU) |
| :--- | :---: | :---: |
| **BUSI** | `[ 0.000 ]` | `[ 0.000 ]` |
| **BUSBRA** | `[ 0.000 ]` | `[ 0.000 ]` |

*(Note: Replace the bracketed placeholders with your final evaluation metrics)*

---

## 🔬 Error Analysis

To build trust in medical AI, we need to know exactly where the model struggles. Our error mapping visualizes the network's decision boundaries directly against the ground truth.

> **[🖼️ UPLOAD ERROR ANALYSIS IMAGE HERE]**  
> *(Drag and drop your generated error map visual right here)*

![Error Analysis Map](link_to_error_analysis_image.png)

* ⬜ **Pure White:** True Positives *(Spot-on tissue identification)*
* 🟥 **Crimson Red:** False Positives *(Background hallucinated as a tumor / Over-segmentation)*
* 🟦 **Deep Blue:** False Negatives *(Missed tumor regions / Under-segmentation)*

---

## 🧠 Model Interpretability (Grad-CAM)

We don't just want a black box. Using Gradient-weighted Class Activation Mapping (Grad-CAM), we peek into the network's "mind" to ensure it is focusing on true pathological features rather than irrelevant image artifacts.

> **[🖼️ UPLOAD GRAD-CAM IMAGE HERE]**  
> *(Drag and drop your Grad-CAM overlay heatmap right here)*

![Grad-CAM Heatmap Visualization](link_to_gradcam_image.png)

---

## ✍️ Authors

* **Rounak Saha** 
* **[Co-Author Name]**
* **[Co-Author Name]**
