# 🌾 Rice Leaf Disease Prediction

This project aims to classify rice leaf diseases using a **Convolutional Neural Network (CNN)** model.  
It identifies three major diseases affecting rice plants:

- **Leaf Blast**
- **Bacterial Blight**
- **Brown Spot**

---

## 📘 Project Overview

This project demonstrates how deep learning can be applied to agriculture to automate the detection of rice leaf diseases.  
The workflow includes **data preprocessing**, **model building**, **training**, **evaluation**, and **prediction**.

---

## 🧩 Workflow

| Step | Description |
|------|--------------|
| 1. Data Collection | Gather and label images of rice leaves |
| 2. Preprocessing | Resize, normalize, and split images into train/test sets |
| 3. Build CNN | Define a convolutional neural network architecture |
| 4. Compile | Configure optimizer, loss, and evaluation metrics |
| 5. Train | Fit the CNN on training data |
| 6. Evaluate | Measure performance using accuracy and confusion matrix |
| 7. Predict | Test on unseen rice leaf images |

---

## 🧠 Model Architecture

A **Convolutional Neural Network (CNN)** was used with the following layers:

- Base Model:Convolutional + MaxPooling layers for feature extraction  
- Dropout layers: for regularization  
- Fully Connected Layers: for classification  
- Output Layer: softmax activation (for 3-class classification)

A **Transfer Learning** was used with the following layers:

- Base Model: MobileNetV2 (pre-trained on ImageNet) used for feature extraction.
- Frozen Layers: The convolutional base is frozen to retain pre-trained weights.
- Fully Connected Layers: for classification
- Dropout layers: for regularization 
- Output Layer: softmax activation (for 3-class classification)

---

## 📊 Evaluation Metrics

The model is evaluated using:

- **Accuracy**
- **Confusion Matrix**
- **Classification Report** (Precision, Recall, F1-Score)

---

## 🛠️ Installation & Usage

### 1️⃣ Clone this repository
```bash
git clone https://github.com/K-m-jesferali/Rice-leaf-Disease-Prediction.git
cd Rice-Leaf-Disease-Prediction
```

### 2️⃣ Install dependencies
```bash
pip install -r requirements.txt
```

### 3️⃣ Run the notebook
Open `Rice_leaf.ipynb` in Jupyter Notebook or VS Code and execute the cells step-by-step.

---

## 📂 Dataset

The dataset contains images of rice leaves categorized into three disease classes.  
Each image is preprocessed by resizing and normalization before training.

---

## 📈 Results

The trained CNN model achieves high classification accuracy in detecting rice leaf diseases.  
Performance metrics are visualized using accuracy and loss curves along with a confusion matrix.

---

## 💾 Model Saving

The trained model is saved in `.h5` format and can be loaded for future predictions.

---

## 👨‍💻 Author

**Mohamed Jesfer Ali K**  
📧 kmjesferali2003@gmail.com  
📍 India  

---

## 🏁 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

