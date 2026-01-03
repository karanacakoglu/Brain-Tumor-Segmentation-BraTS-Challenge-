# 🧠 BraTS: Brain Tumor Segmentation with UNet & ResUNet

### Project Overview
Medical image segmentation is a critical task in neuro-oncology. This project explores the implementation of **UNet** and **ResUNet** architectures to segment brain tumors from multi-modal MRI scans. Based on the **BraTS (Brain Tumor Segmentation)** challenge, the goal is to provide high-precision masks for different tumor regions.

---

### 📊 Dataset & Modalities
The project utilizes multi-modal MRI data, which is essential for defining tumor boundaries:
* **T1 & T1-weighted Contrast-Enhanced (T1ce)**
* **T2-weighted**
* **FLAIR (Fluid Attenuated Inversion Recovery)**

---

### 🛠️ Technical Implementation (Work in Progress)
This repository documents the ongoing development of the segmentation pipeline:

* **Encoder-Decoder Architecture:** Implementing a classic **UNet** backbone for feature contraction and symmetrical expansion.
* **Residual Connections:** Integrating **ResNet** blocks (ResUNet) to facilitate deeper feature learning and mitigate the vanishing gradient problem in 3D-like contexts.
* **Custom Metrics:** Since medical masks occupy a small fraction of the image, the training focuses on **Dice Coefficient** instead of standard pixel accuracy.
* **Framework:** Developing with **PyTorch / TensorFlow** to handle custom training loops for medical tensors.

---

### 🚧 Current Challenges & Next Steps
- [ ] Completing the data loader for large 3D NIfTI files.
- [ ] Fine-tuning skip connections between the encoder and decoder.
- [ ] Finalizing the evaluation on the validation set.

---

### 🔗 Resources
- **Dataset:** [BraTS Challenge Info](https://www.med.upenn.edu/cbica/brats-2021/)
- **Frameworks:** Python, PyTorch(Scratch), NiBabel (for NIfTI files
- **Colab links:**
* **BraTS-UNet3d Colab link: [UNet3d](https://colab.research.google.com/drive/1OodJB_JVhr42KtSpJCytY2q6bkIE7lF4?authuser=1&usp=drive_open)**
* **BraTS-ResUNet3d Colab link: [ResNet3d Hyper](https://colab.research.google.com/drive/1EjjpdgcD22ax8XBGNmqegFX9m26krqgI?authuser=1&usp=drive_open)**
