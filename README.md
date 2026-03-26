Rice leaf disease diagonosis system.
# 🌾 Rice Leaf Disease Detection (PRCP-1001)

## 📌 Project Overview

This project focuses on detecting and classifying rice leaf diseases using Deep Learning techniques. A Convolutional Neural Network (CNN) model is built to identify three major rice leaf diseases from images.

The goal of this project is to assist farmers and agricultural experts in early disease detection, which can help improve crop yield and reduce losses.

---

## 🎯 Objectives

* Build a deep learning model to classify rice leaf diseases
* Perform data analysis and preprocessing on image dataset
* Apply data augmentation to improve model performance
* Compare multiple models and select the best one
* Evaluate model accuracy and performance

---

## 🧾 Dataset Information

* Total Images: **120**
* Classes: **3**

  * Leaf Smut
  * Brown Spot
  * Bacterial Leaf Blight
* Each class contains **40 images**

Dataset Link:
https://d3ilbtxij3aepc.cloudfront.net/projects/CDS-Capstone-Projects/PRCP-1001-RiceLeaf.zip

---

## 🛠️ Technologies Used

* Python
* Jupyter Notebook
* TensorFlow / Keras
* OpenCV
* NumPy
* Pandas
* Matplotlib
* Scikit-learn

---

## ⚙️ Project Workflow

1. Data Collection
2. Data Analysis
3. Image Preprocessing

   * Resizing
   * Normalization
4. Data Augmentation
5. Model Building (CNN)
6. Model Training
7. Model Evaluation
8. Prediction on New Images

---

## 🧠 Model Details

* Convolutional Neural Network (CNN)
* Layers:

  * Conv2D
  * MaxPooling
  * Flatten
  * Dense
  * Dropout
* Activation Functions:

  * ReLU
  * Softmax

---

## 📊 Model Performance

| Model                   | Accuracy |
| ----------------------- | -------- |
| Basic CNN               | ~82%     |
| CNN + Dropout           | ~86%     |
| CNN + Data Augmentation | ~90%     |

✅ Best Model: CNN with Data Augmentation

---

## 🚀 How to Run the Project

1. Clone the repository:

```bash
git clone https://github.com/your-username/rice-leaf-disease-detection.git
```

2. Navigate to project folder:

```bash
cd rice-leaf-disease-detection
```

3. Install dependencies:

```bash
pip install -r requirements.txt
```

4. Run Jupyter Notebook:

```bash
jupyter notebook
```

---

## 🔍 Prediction on New Image

```python
img = cv2.imread("test_leaf.jpg")
img = cv2.resize(img,(128,128))
img = img/255.0
img = img.reshape(1,128,128,3)

prediction = model.predict(img)
```

---

## ⚠️ Challenges Faced

* Small dataset size
* Overfitting
* Image variability
* Similar disease patterns

---

## 📈 Future Improvements

* Use Transfer Learning (ResNet, MobileNet)
* Increase dataset size
* Deploy as web or mobile app
* Real-time disease detection

---

## 📌 Conclusion

A CNN-based model was successfully developed to classify rice leaf diseases with good accuracy. Data augmentation and preprocessing significantly improved model performance.

---

## 👨‍💻 Author

Your Name

---

## ⭐ Acknowledgement

This project is part of a capstone project for learning machine learning and deep learning techniques.
