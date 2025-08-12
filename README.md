# 🐾 Animal Image Classification with Grad-CAM Visualization

This project is an **Animal Image Classification** system built using **Deep Learning** and **Transfer Learning** with **MobileNetV2**.  
It can upload an image, classify it into animal categories, and generate **Grad-CAM heatmaps** to visualize which parts of the image influenced the model's decision.  

## 🚀 Features
- **Image Classification** using a fine-tuned MobileNetV2 model.
- **Data Augmentation** to improve model generalization.
- **Two-Phase Training**:
  - Initial training with frozen base layers.
  - Fine-tuning with all layers trainable.
- **Explainable AI** with Grad-CAM integration for model interpretability.
- **Performance Optimization** using callbacks:
  - EarlyStopping
  - ReduceLROnPlateau
  - ModelCheckpoint
- Clean modular code structure for easy customization.

---

## 🛠️ Tech Stack
- **Programming Language:** Python
- **Deep Learning Framework:** TensorFlow / Keras
- **Model Architecture:** MobileNetV2 (Transfer Learning)
- **Visualization:** Matplotlib, OpenCV
- **Explainability:** Grad-CAM

---


---

## 📊 How It Works
1. **Data Loading & Preprocessing**
   - Images are resized to **160x160** and normalized.
   - Data augmentation is applied to the training set.
   
2. **Model Architecture**
   - Base model: **MobileNetV2** (ImageNet weights).
   - Additional layers: Global Average Pooling, Dense, BatchNorm, Dropout, Softmax.
   
3. **Training**
   - Phase 1: Train only top layers.
   - Phase 2: Unfreeze all layers and fine-tune with a lower learning rate.
   
4. **Grad-CAM Visualization**
   - Generates a heatmap highlighting regions that influenced the classification.

---

## 📸 Example Grad-CAM Output
| Original Image | Grad-CAM Heatmap |
|----------------|------------------|
| ![Animal](test_images/sample.jpg) | ![Grad-CAM](gradcam_result.jpg) |

---

## 📈 Model Performance
- Validation Accuracy: **~93%** *(replace with your result)*
- Loss & accuracy plots can be generated to visualize training progress.

---

## 🖥️ Installation & Usage

### 1️⃣ Clone Repository
```bash
git clone https://github.com/Ishat1426/Animal-classification-gradcam.git
cd Animal-classification-gradcam

## 🖥️ To RUN IT
OPEN THE TERMIAL AND TYPE python app.py
