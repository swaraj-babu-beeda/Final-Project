# 🧠 Hybrid Quantum–Classical Model for Retinal Disease Detection

Early detection of retinal diseases can save vision.  
This project implements a **Hybrid Quantum–Classical Machine Learning pipeline** that classifies retinal fundus images into four categories:  

- 👁️ **Normal**  
- ⚠️ **Diabetic Retinopathy**  
- 🔬 **Glaucoma**  
- 🌫️ **Cataract**

We combine a **Convolutional Neural Network (CNN)** feature extractor with a **PennyLane Variational Quantum Classifier** to explore whether quantum layers improve classification performance and interpretability.

---

## 🚀 Results (Validation Set)

| Metric          | Value |
|-----------------|-------|
| Accuracy        | XX%   |
| Precision (avg) | XX%   |
| Recall (avg)    | XX%   |
| F1-Score (avg)  | XX%   |

📊 *See the [Colab notebook](#-colab-notebook) for detailed classification reports and confusion matrix.*

---

## 🗂️ Dataset

- Source: [Public Retinal Fundus Dataset](<add link here>)  
- Classes: 4 (Normal, Glaucoma, Diabetic Retinopathy, Cataract)  
- Preprocessing:
  - Normalization and resizing  
  - Data augmentation (flip, rotation, zoom)  
  - Label encoding  

⚠️ *This dataset is for **research/educational purposes only** — not clinical deployment.*

---

## 🏗️ Model Architecture

**Pipeline**:  
1. **CNN (Keras/TensorFlow)** → Extract features  
2. **Quantum Layer (PennyLane)** → Variational classifier  
3. **Classical Optimizer** → Cross-entropy minimization  

🖼️ *Architecture diagram here (replace with image)*  

---

## 📓 Colab Notebook

Run the full pipeline interactively in Google Colab:  
👉 [Open in Colab](<insert your Colab link here>)  

---

## ⚙️ Installation (Local)

Clone the repo:

```bash
git clone https://github.com/swaraj-babu-beeda/Final-Project.git
cd Final-Project
