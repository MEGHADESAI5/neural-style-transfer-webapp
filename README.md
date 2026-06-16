# 🎨 Neural Style Transfer Web Application (AdaIN)

An end-to-end Deep Learning and Computer Vision project that performs artistic style transfer using **Adaptive Instance Normalization (AdaIN)**. The application allows users to blend the content of one image with the artistic style of another while preserving structural details and generating visually appealing results in real time.

## 🌐 Live Demo

https://huggingface.co/spaces/Megha5/Neural_Style_Transfer

---

## 🚀 Features

* Upload custom content and style images
* Real-time neural style transfer
* Adjustable style intensity using alpha blending
* AdaIN-based feature alignment
* VGG-19 feature extraction network
* High-quality image generation
* Interactive Gradio web interface
* Cloud deployment using Hugging Face Spaces

---

## 🧠 Technology Stack

### Machine Learning & Deep Learning

* Python
* PyTorch
* TorchVision

### Computer Vision

* Neural Style Transfer (NST)
* Adaptive Instance Normalization (AdaIN)
* Feature Extraction using VGG-19

### Deployment & Interface

* Gradio
* Hugging Face Spaces

---

## 🏗️ System Architecture

Content Image
↓
VGG-19 Encoder
↓
Content Features

Style Image
↓
VGG-19 Encoder
↓
Style Features

Content Features + Style Features
↓
Adaptive Instance Normalization (AdaIN)
↓
Decoder Network
↓
Stylized Output Image

---

## 🔬 How It Works

### 1. Content Feature Extraction

The content image is passed through a pretrained VGG-19 encoder to extract high-level semantic features that represent image structure and object layouts.

### 2. Style Feature Extraction

The style image is encoded using the same VGG-19 network to capture texture, color distribution, and artistic patterns.

### 3. Adaptive Instance Normalization (AdaIN)

AdaIN aligns the mean and standard deviation of content features with those of style features, effectively transferring artistic characteristics while preserving image content.

AdaIN Formula:

AdaIN(x, y) = σ(y) × ((x − μ(x)) / σ(x)) + μ(y)

Where:

* x = Content Features
* y = Style Features
* μ = Mean
* σ = Standard Deviation

### 4. Image Reconstruction

A decoder network reconstructs the transformed features into a stylized image.

---

## 📂 Project Structure

```text
Neural_Style_Transfer/
│
├── app.py
├── requirements.txt
├── vgg_normalised.pth
├── decoder_50.pth
├── models.py
├── utils.py
└── README.md
```

---

## 📈 Key Concepts Demonstrated

* Deep Learning
* Computer Vision
* Convolutional Neural Networks (CNNs)
* Transfer Learning
* Feature Space Manipulation
* Image Generation
* Neural Style Transfer
* Model Deployment
* Interactive AI Applications

---

## 🎯 Learning Outcomes

Through this project, I gained hands-on experience in:

* Designing and deploying deep learning applications
* Working with pretrained neural networks
* Understanding feature representations in CNNs
* Implementing AdaIN-based style transfer
* Building user-facing AI applications with Gradio
* Deploying machine learning projects to the cloud

---

## 👩‍💻 Author

**Megha Desai**
B.E. Computer Science Engineering (CSE '27)

Aspiring AI/ML Engineer | Deep Learning | Computer Vision | Generative AI | Python | PyTorch


