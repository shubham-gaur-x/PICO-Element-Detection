# NLP Modeling Project - Milestone 5

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
# Save this file as README.md in your project directory

# Commit and push to GitHub
git add README.md
git commit -m "Added README with model download instructions"
git push origin main
```
