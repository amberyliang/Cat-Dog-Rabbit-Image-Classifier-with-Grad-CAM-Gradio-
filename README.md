# 🐾 Cat-Dog-Rabbit Image Classifier (with Grad-CAM & Gradio)

A lightweight deep learning project for **multiclass image classification** of cats 🐱, dogs 🐶, and rabbits 🐰 — built with TensorFlow and deployed through an intuitive **Gradio** web interface.

---

### 📌 Features

* ✅ Image classification using pretrained **MobileNetV2** with fine-tuning
* ✅ Support for **Grad-CAM** to visualize model attention
* ✅ **Unknown detection** when confidence is too low
* ✅ **Gradio UI** for interactive web app with:

  * Single image upload
  * Batch prediction (.jpg/.png)
  * Live webcam capture (mobile/desktop)
* ✅ Mobile-friendly and notebook-compatible (Google Colab)

---

### 📂 Dataset Format

Please prepare your dataset using the following folder structure:

```
dataset/
├── train/
│   ├── cat/
│   ├── dog/
│   └── rabbit/
└── val/
    ├── cat/
    ├── dog/
    └── rabbit/
```

* Images should be placed inside the respective class folders.
* Recommended total: \~1500 images or more for training.

---

### ⚙️ Tech Stack

| Component              | Description                                        |
| ---------------------- | -------------------------------------------------- |
| `TensorFlow 2.x`       | Deep learning framework                            |
| `MobileNetV2`          | Lightweight pretrained model for transfer learning |
| `Grad-CAM`             | Model interpretability visualization               |
| `Gradio`               | Interactive web interface for inference            |
| `OpenCV`               | Image handling and preprocessing                   |
| `Matplotlib / Seaborn` | Metrics visualization                              |

---

### 🚀 How to Use (on Google Colab)

1. Open `cat-dog-rabbit-classifier.ipynb` on Colab
2. Upload your dataset to Google Drive
3. Run all cells to train or load model
4. Enjoy the Gradio interface for image classification!

---

### 🧠 Model Behavior

* The model returns the top-3 predicted classes with confidence scores
* If the model’s confidence is below a set threshold (default `0.6`), it returns:

  ```
  Unknown / 非貓狗兔: 1.0
  ```

---

### 📷 Web Demo Interface (Gradio Tabs)

* `單張圖片預測` – Upload one image, see prediction and Grad-CAM
* `多圖批次預測` – Upload multiple images and see predictions
* `拍照即時辨識` – Capture image using webcam (supports mobile camera)

---

### 📝 Future Work

* Model performance comparison (MobileNet vs EfficientNet)
* Entropy-based uncertainty estimation
* Automatic CSV export of predictions
* Deploy to Hugging Face Spaces for permanent access

---

### 👩‍💻 Author

Created by \[Yu-Jung,Liang].
This project was built for academic exploration, UI/UX research, and computer vision prototyping.

---

### 📄 License

This repository is released under the MIT License. Free for educational and research purposes.
