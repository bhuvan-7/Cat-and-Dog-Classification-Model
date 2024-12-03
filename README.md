# 🐾 Cat vs. Dog Image Classifier 🐾

This project is a deep learning-based image classification model that identifies whether an uploaded image is of a cat or a dog. The model is trained on a dataset of 22k+ images and deployed using Flask, with a user-friendly HTML front-end interface.

---

## 📋 Table of Contents
- [📖 Introduction](#-introduction)
- [✨ Features](#-features)
- [⚙️ Technologies Used](#%EF%B8%8F-technologies-used)
- [📂 Dataset Description](#-dataset-description)
- [🧠 Model Training](#-model-training)
- [🌐 Deployment](#-deployment)
- [📊 Results and Accuracy](#-results-and-accuracy)
- [🔮 Future Enhancements](#-future-enhancements)
- [🤝 Contributing](#-contributing)
- [📜 License](#-license)
- [🚀 How to Run the Project](#-how-to-run-the-project)

---

## 📖 Introduction

This project uses Convolutional Neural Networks (CNNs) to classify images into two categories: cats and dogs. The model is trained and evaluated on a dataset of 22,000+ labeled images and is capable of providing predictions in a deployed Flask application.

---

## ✨ Features

- **High Accuracy**: Achieved 95%+ validation accuracy during training.
- **Real-Time Prediction**: Upload an image and instantly classify it as a cat or a dog.
- **Responsive UI**: A visually appealing web interface with a black and red theme.
- **Confidence Thresholding**: Rejects predictions when the confidence is too low.

---

## ⚙️ Technologies Used

- **Programming Languages**: Python, HTML, CSS
- **Libraries and Frameworks**:
  - TensorFlow/Keras for building and training the CNN
  - Flask for deploying the model
  - NumPy and Matplotlib for data preprocessing and visualization
- **Frontend**: HTML5, CSS3 with Bootstrap
- **Deployment Platform**: Flask (can be hosted on platforms like Heroku, AWS, or Google Cloud)

---

## 📂 Dataset Description

- **Source**: Kaggle's Cats and Dogs Dataset
- **Total Images**: 22,000+
  - Cats: 11,000+
  - Dogs: 11,000+
- **Splits**:
  - **Training**: 70%
  - **Validation**: 15%
  - **Testing**: 15%

Dataset preprocessing involves resizing the images to 150x150 pixels and normalizing the pixel values to the range [0, 1].

---

## 🧠 Model Training

The model is built using a CNN architecture with the following layers:

- **Convolutional Layers**: Extract spatial features from the images.
- **MaxPooling Layers**: Downsample feature maps.
- **Dense Layers**: Fully connected layers for classification.
- **Output Layer**: Binary classification using a sigmoid activation function.

**Hyperparameters**:
- **Optimizer**: Adam
- **Loss Function**: Binary Crossentropy
- **Batch Size**: 32
- **Epochs**: 15

---

## 🌐 Deployment

The project is deployed using Flask, with an interactive front-end where users can upload an image to classify it. The interface includes:

- A drag-and-drop file upload option
- Real-time predictions with confidence scores
- A visually appealing black-and-red theme

---

## 📊 Results and Accuracy

- **Training Accuracy**: ~95%
- **Validation Accuracy**: ~93%
- **Inference Time**: ~2 seconds per image

| **Metric**      | **Value** |
|------------------|-----------|
| **Precision**    | 0.94      |
| **Recall**       | 0.92      |
| **F1 Score**     | 0.93      |

---

## 🔮 Future Enhancements

- **Add "Unknown" Category**: Improve model robustness by rejecting non-cat/dog images.
- **Integrate Transfer Learning**: Use pre-trained models (e.g., ResNet) for better performance.
- **Deploy on Cloud**: Host the application on platforms like Heroku or AWS for global access.

---

## 🤝 Contributing

Contributions are welcome! Please follow these steps:

1. Fork the repository.
2. Create a new branch for your feature/bug fix.
3. Commit your changes and push the branch.
4. Create a pull request describing your changes.

---

## 📜 License

This project is licensed under the [MIT License](LICENSE).

---

## 🚀 How to Run the Project

### 1. Clone the Repository
```bash
git clone https://github.com/your-username/cat-dog-classifier.git
cd cat-dog-classifier
