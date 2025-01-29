# NLP Modeling Project - Milestone 5

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

# Save this file as README.md in your project directory

# Commit and push to GitHub
git add README.md
git commit -m "Added README with model download instructions"
git push origin main
