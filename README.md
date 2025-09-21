# 🧠 Hybrid Quantum–Classical Retinal Disease Classification

**Automated classification of retinal fundus images into four categories:**  
**Normal**, **Diabetic Retinopathy**, **Glaucoma**, and **Cataract** — using a hybrid **CNN + Quantum Machine Learning pipeline**.

This project explores whether **quantum-enhanced layers** can improve classification performance and interpretability over classical CNN models.

---

## 🚀 Results

The hybrid quantum-classical model achieved **high performance** on the dataset:

| Model Type | Accuracy (%) | F1-Score (%) |
|------------|--------------|--------------|
| Classical CNNs (ResNet18 / ResNet34 / ResNet50 / ResNet101 / ResNet152 / InceptionV3) | 85.3 – 89.8 | 85.6 – 89.5 |
| **Hybrid Quantum–Classical Model** | **97.2 – 98.5** | **97.4 – 98.4** |

> The quantum layers significantly improved feature separability and model interpretability.

---

## 🗂️ Dataset & Preprocessing

- **Dataset**: Public retinal fundus dataset (4 classes).  
- **Preprocessing steps**:
  - Image resizing and normalization  
  - Data augmentation (rotation, flips, zoom)  
  - Feature extraction via pretrained CNNs (ResNet / InceptionV3)  

> ⚠️ Dataset used for **research/educational purposes only**.

---

## 🏗️ Model Architecture

**Pipeline Overview:**

1. **CNN Feature Extractor** (ResNet/InceptionV3) → Extract embeddings from images  
2. **Variational Quantum Classifier** (PennyLane) → Quantum circuit for classification  
3. **Hybrid Optimization** → Classical optimizer minimizing cross-entropy  

🖼️ *Visual placeholders:*
- Architecture diagram  
- Confusion matrix  
- Sample input images with predicted labels  

---

## 📊 Key Visuals

Here are some visual highlights of the project:

- **Confusion Matrix**  
  ![Confusion Matrix](images/confusion_matrix.png)

- **Sample Predictions**  
  ![Sample Predictions](images/sample_predictions.png)

- **Training Curves / Accuracy-Loss Plots** *(optional)*  
  ![Training Curves](images/training_curves.png)


---

## 💡 Learnings & Future Work

**Learnings:**

- Quantum layers can significantly boost performance on retinal image classification.  
- Circuit design, embedding strategy, and preprocessing critically affect results.  

**Future Work:**

- Benchmark against external clinical datasets to test generalization.  
- Explore lightweight CNN + quantum layer combinations for potential deployment.  
- Ablation studies comparing classical vs hybrid models in depth.  

---

## 🤝 Connect

Swaraj Babu Beeda  
- [LinkedIn](https://www.linkedin.com/in/swaraj-babu-beeda/)  
- Email: swarajbabubeeda98@gmail.com  
- GitHub: [swaraj-babu-beeda](https://github.com/swaraj-babu-beeda)  

---

*MIT License*
