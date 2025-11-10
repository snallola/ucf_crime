# 🧠 Human Activity Recognition using Deep Learning

This project implements a **Deep Learning-based multi-class classification model** designed to recognize and differentiate between various human activities such as **Abuse, Arrest, Shoplifting**, and other behavioral actions using video frame data.

---

## 🏗️ Model Description

The model utilizes a **Convolutional Neural Network (CNN)** built with **TensorFlow/Keras** for spatial feature extraction and classification.  
Each input frame is **preprocessed (resized, normalized, tensorized)** and passed through multiple convolutional and pooling layers before classification.

**Key Components:**
- **Convolutional Layers:** Extract visual and motion-related features.
- **Activation (ReLU):** Introduce non-linearity.
- **Pooling Layers:** Reduce dimensionality and prevent overfitting.
- **Flatten + Dense Layers:** Map learned features to class probabilities.
- **Output Layer (Softmax):** Generates final activity predictions.

---

## ⚙️ Training Strategy

The model was trained using **5-Fold Cross Validation** to ensure reliability and generalization.  
Each fold trains on 80% of the data and validates on the remaining 20%, rotating until all subsets are tested.

---

## 📈 Performance Metrics

### **1️⃣ Training vs Validation Accuracy**
![Training vs Validation Accuracy](outputs/Final_outputs.pdf)

- Accuracy steadily increases across all folds.
- Both training and validation curves align closely → minimal overfitting.
- Final accuracy reaches near 95–100% across all folds.

---

### **2️⃣ Training vs Validation Loss**
![Training vs Validation Loss](outputs/Final_outputs.pdf)

- Loss decreases rapidly and stabilizes at a low value.
- Similar convergence trends across folds indicate consistent model learning.
- Confirms robust feature extraction and stable optimization.

---

### **3️⃣ Confusion Matrix**
![Confusion Matrix](outputs/CM_outputs.pdf)

- Diagonal dominance shows most actions correctly classified.
- Minor off-diagonal confusion only between visually similar actions.
- Indicates strong performance and reliable behavior detection.

---

### **4️⃣ Sample Predictions**
![Sample Predictions](outputs/Final_outputs.pdf)

- Displays the model’s real-time classification output on video frames.
- Demonstrates correct recognition of activities such as *Shoplifting* or *Abuse*.
- Validates the practical deployment potential in surveillance contexts.

---

## 🧮 Performance Summary

| Metric | Average (Across 5 Folds) |
|---------|--------------------------|
| Accuracy | 0.99 |
| Precision | High |
| Recall | High |
| F1-Score | Excellent |

---

## 💡 Why This Model Works Well
- CNN layers capture spatial and motion cues essential for human activity recognition.  
- 5-Fold validation ensures stability and robustness.  
- Real-world frames enable adaptation to natural lighting and environment variations.

---

## 📊 Future Improvements
- Integrate **temporal modeling (LSTM/3D CNNs)** for continuous action recognition.
- Deploy as a real-time **surveillance or safety monitoring system**.
- Expand dataset with more complex activity types.

---

## 🧑‍💻 Developed Using
- **TensorFlow / Keras**
- **OpenCV**
- **Python 3.10**
- **Matplotlib / NumPy / Pandas**

---

## 🏁 Conclusion

This project demonstrates the effectiveness of a CNN-based system in identifying human actions from real-world video data.  
Its high accuracy and strong validation results make it suitable for **security, retail analytics, and behavioral monitoring** applications.

---

