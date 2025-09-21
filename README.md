# Hybrid Quantum–Classical Retinal Disease Classification

**Hybrid Quantum-Classical ML model that classifies retinal fundus images into 4 classes** — Normal, Diabetic Retinopathy, Glaucoma, Cataract — combining classical CNN feature extractors (ResNet / Inception-V3) with a PennyLane variational quantum classifier.  
Achieved **~97-98% accuracy** & **~97-98% F1-score** using the hybrid model.  

---

## 🚀 Results Summary

| Model Type | Accuracy (%) | F1-Score (%) |
|-------------|----------------|----------------|
| Classical CNNs (ResNet18 / ResNet34 / ResNet50 / ResNet101 / ResNet152 / InceptionV3) | **85.3 – 89.8** | **85.6 – 89.5** |
| **Hybrid Quantum-Classical (Quantum Classifier on top of same feature extractors)** | **97.2 – 98.5** | **97.4 – 98.4** |

---

## 🗂️ Dataset & Preprocessing

- **Dataset**: Public retinal fundus image dataset (4 classes: Normal, Diabetic Retinopathy, Glaucoma, Cataract)  
- Preprocessing steps:
  - Resize / normalize images  
  - Data augmentation (flips, rotations, zoom etc.)  
  - Split into training & validation sets  
- Feature extraction was done via pretrained CNNs (ResNet variants, InceptionV3), with the last layer removed for embedding → to feed quantum classifier.

---

## 🏗️ Model Architecture

1. Classical CNN (feature extraction) using variants: ResNet18, ResNet34, ResNet50, ResNet101, ResNet152, and InceptionV3  
2. Variational Quantum Classifier built using PennyLane quantum circuits (utilizing gates like Hadamard, CNOT etc.)  
3. Training loop: classical optimizer minimizing cross-entropy loss on the hybrid model  

---

## 📓 Notebooks & Interactive Runs

You can run the full pipeline via the Colab / Jupyter notebook: `final_mini_project.ipynb`  
This includes preprocessing, feature extraction, quantum circuit implementation, and evaluation.  

---

## ⚙️ Setup (Local / Reproduce)

```bash
git clone https://github.com/swaraj-babu-beeda/Final-Project.git
cd Final-Project
# ensure Python ≥ 3.8, install dependencies
pip install -r requirements.txt
jupyter notebook final_mini_project.ipynb
