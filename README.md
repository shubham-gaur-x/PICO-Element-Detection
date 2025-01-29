# NLP Modeling Project - Milestone 5

<<<<<<< Updated upstream
=======
<<<<<<< HEAD
This project is a Named Entity Recognition (NER) and Text Classification System built using deep learning models trained on PubMed abstracts. The system utilizes BiLSTM, FFNN, and Transformer-based architectures to process text efficiently.

---

## Features

- **Fast Inference**: Optimized models for real-time predictions.
- **Custom Model**: Trained on medical abstracts for precise entity recognition.
- **User-Friendly Interface**: Easy-to-use implementation for deployment.
- **Google Drive Integration**: Downloads required model files automatically.

---

## Table of Contents

- [Demo](#demo)
- [Setup Instructions](#setup-instructions)
- [Project Structure](#project-structure)
- [How It Works](#how-it-works)
- [Technologies Used](#technologies-used)
- [License](#license)

---

## 🛠 Setup Instructions

Follow these steps to set up and run the project locally:

### Prerequisites

- Python **3.8 or higher**
- **Git**

### Installation

#### 1. Clone the Repository:
```bash
git clone https://github.com/shubham-gaur-x/NLP-Modeling-Project.git
cd NLP-Modeling-Project
```

#### 2. Install Dependencies:  
Install the required Python libraries from `requirements.txt`:
```bash
pip install -r requirements.txt
```

#### 3. Download Model Files:  
The model and tokenizer files are hosted on Google Drive. The app will **automatically download them** when you run it for the first time. Ensure you have an internet connection.

- **Model**: [model.onnx](https://drive.google.com/file/d/your_model_link_here)
- **Tokenizer**: [tokenizer.json](https://drive.google.com/file/d/your_tokenizer_link_here)
- **Config**: [config.json](https://drive.google.com/file/d/your_config_link_here)

#### 4. Run the App:  
Launch the application:
```bash
streamlit run qa_app.py
```

#### 5. Open the app in your browser at:  
```
http://localhost:8501
```

---

## 📂 Project Structure

```bash
NLP-Modeling-Project/
│── qa_app.py               # Main application file
│── requirements.txt        # Python dependencies
│── README.md               # Project documentation
│── medical_text.csv        # Dataset (Medical abstracts)
│── nlp_model/              # Model directory (auto-downloaded files)
│   ├── model.onnx          # ONNX model
│   ├── tokenizer.json      # Tokenizer file
│   ├── config.json         # Model configuration
```

---

## 🔎 How It Works

1️⃣ **User Input:**
   - The user enters a text input for entity recognition.

2️⃣ **Preprocessing:**
   - The text is tokenized using the Hugging Face tokenizer.

3️⃣ **Model Inference:**
   - The tokenized input is processed by the trained ONNX model.

4️⃣ **Entity Extraction:**
   - The model predicts the entity categories within the text.

---

## 🛠 Technologies Used

- **Python**: Core programming language
- **Hugging Face Transformers**: NLP model implementation
- **ONNX Runtime**: Optimized model inference
- **Streamlit**: Web app interface
- **Google Drive API**: Model storage and retrieval

---

## 📜 License

This project is open-source and available under the **MIT License**.

---

## 💡 Contributions

We welcome contributions! Feel free to **fork the repository**, submit **pull requests**, or open **issues** for discussions.

---

## ⬆️ Final Steps to Upload This to GitHub

```bash
=======
>>>>>>> Stashed changes
## 📌 Overview
This project focuses on **Named Entity Recognition (NER) and text classification** using deep learning models.  
We utilize **PubMed abstracts** and implement models like **BiLSTM, FFNN, and Transformer-based architectures**.

## 📂 Model Checkpoints
Due to GitHub's file size limitations, all trained model files are available on **Google Drive**.  

📥 **[Download Model Checkpoints](https://drive.google.com/drive/folders/1-nB8bQW0aQ5WoaExIzxcWo6PnhXkoLiB?usp=sharing)**  

```bash
# 📥 Download & Use the Models

# Step 1: Create a directory for models
mkdir models
cd models

# Step 2: Move downloaded model files here

# Step 3: Load them in Python
import torch
from transformers import AutoModel

# Load BiLSTM Model
bilstm_model = torch.load("models/BiLSTM_model.pth")

# Load Transformer-based Model
transformer_model = AutoModel.from_pretrained("models/distilbert_student_model")

# 🔧 Installation

# Create a virtual environment (optional but recommended)
python -m venv nlp_env
source nlp_env/bin/activate  # On Windows use: nlp_env\Scripts\activate

# Install dependencies
pip install -r requirements.txt

# 🚀 Running Inference

# Run inference using the BiLSTM model
python inference.py --model_path models/BiLSTM_model.pth

# 📜 Repository Structure

NLP_Modeling_Project/
│── models/  (Download models from Drive and store here)
│── notebooks/
│   ├── IE7500_Group3_Mile5_Modeling.ipynb
│   ├── IE7500_NLP_Group3_Mile5_ModelTest_FV.ipynb
│   ├── IE7500_NLP_Group3_PICO_Milestone5.ipynb
│── reports/
│   ├── IE7500_NLP_Group3_Mile5_Models_FV.pdf
│   ├── IE7500_NLP_Group3_Mile6_ModelTest_FV2.pdf
│   ├── IE7500_NLP_Group3_PICO_Milestone5.pdf
│── inference_results.csv
│── requirements.txt
│── README.md  (This file)

# 📥 Alternative: Automated Model Download

# Step 1: Install `gdown` (if not installed)
pip install gdown

# Step 2: Run the script to download models automatically
bash download_models.sh

# Script: download_models.sh
#!/bin/bash
echo "Downloading model files..."
gdown --folder "https://drive.google.com/drive/folders/1-nB8bQW0aQ5WoaExIzxcWo6PnhXkoLiB?usp=sharing" -O models/
echo "Download complete!"

# ✨ Contributions
# Feel free to fork the repository, submit pull requests, or open issues for discussions.

# 📜 License
# This project is open-source and available under the MIT License.

# Final Steps to Upload This to GitHub

<<<<<<< Updated upstream
=======
>>>>>>> 4875e039e54f88bf1dd1479cbed02249aeb972b5
>>>>>>> Stashed changes
# Save this file as README.md in your project directory

# Commit and push to GitHub
git add README.md
git commit -m "Added README with model download instructions"
git push origin main
<<<<<<< Updated upstream
=======
<<<<<<< HEAD
```
=======
>>>>>>> 4875e039e54f88bf1dd1479cbed02249aeb972b5
>>>>>>> Stashed changes
