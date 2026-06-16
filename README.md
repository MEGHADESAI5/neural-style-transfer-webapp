🎨 Neural Style Transfer Web Application (AdaIN-based)

An AI-powered web application that performs real-time artistic style transfer using Adaptive Instance Normalization (AdaIN). The system blends the content of one image with the style of another while preserving semantic structure and applying artistic textures.

🚀 Features

📤 Upload custom content and style images
🎨 Real-time neural style transfer
⚡ Adjustable style strength (alpha blending)
🧠 Deep learning pipeline using VGG-19 encoder
🔁 AdaIN (Adaptive Instance Normalization) for style alignment
🌐 Lightweight Flask-based web interface
🖼️ High-quality stylized image generation


🧠 Tech Stack

Backend
Python 3.x
Flask (Web Framework)
PyTorch (Deep Learning Framework)
Deep Learning Model
VGG-19 (Pretrained Encoder)
Custom Decoder Network
AdaIN (Adaptive Instance Normalization)

Frontend
HTML5
CSS3
JavaScript (Vanilla)


🏗️ System Architecture
Content Image ───────┐
                     │
                     ▼
              VGG-19 Encoder
                     │
                     ▼
Style Image ───► Feature Extraction
                     │
                     ▼
        Adaptive Instance Normalization (AdaIN)
                     │
                     ▼
              Decoder Network
                     │
                     ▼
            Stylized Output Image



🔬 How It Works
1.Content Encoding
  Input content image is passed through a pretrained VGG-19 encoder
  Extracts high-level feature representations (structure, layout)
2.Style Encoding
  Style image is also encoded using the same VGG features
  Captures texture, color distribution, and artistic patterns
3.AdaIN Layer
  Aligns content feature statistics with style feature statistics

Formula:

AdaIN(x, y) = σ(y) * ((x - μ(x)) / σ(x)) + μ(y)
Where:
x = content features
y = style features
μ = mean, σ = standard deviation
4.Decoder
  Converts transformed features back into image space
  Produces final stylized output



📁 Project Structure

neural-style-transfer/
│
├── static/
│   ├── uploads/
│   └── results/
│
├── templates/
│   └── index.html
│
├── models/
│   ├── encoder.py
│   ├── decoder.py
│   └── adain.py
│
├── utils/
│   └── image_processing.py
│
├── app.py
├── requirements.txt
└── README.md


📌 Key Concepts Used

Deep Feature Extraction (CNNs)
Transfer Learning (VGG-19)
Instance Normalization
Style Transfer (AdaIN)
Image-to-Image Translation
Flask Web Deployment


👨‍💻 Author
Megha Desai
B.E. Computer Science (CSE '27)
Interested in AI/ML, Deep Learning, and Computer Vision