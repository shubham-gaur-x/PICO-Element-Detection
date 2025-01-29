# NLP Modeling Project - Milestone 5

## Overview
This project involves Named Entity Recognition (NER) and text classification using various deep learning models. The dataset consists of PubMed abstracts, and we fine-tuned models like BiLSTM, FFNN, and Transformer-based models.

## Model Checkpoints
Due to GitHub's file size limitations, all trained model files are hosted on **Google Drive**. You can download them from the link below:

📂 **[Download Model Checkpoints](https://drive.google.com/drive/folders/1-nB8bQW0aQ5WoaExIzxcWo6PnhXkoLiB?usp=sharing)**

### **Usage**
After downloading the models, place them in a `models/` directory inside the project folder.

```bash
mkdir models
cd models
# Move downloaded files here
```

Then, load the models in Python:
```python
import torch
from transformers import AutoModel

# Example: Load BiLSTM Model
bilstm_model = torch.load("models/BiLSTM_model.pth")

# Example: Load Transformer-based Model
transformer_model = AutoModel.from_pretrained("models/distilbert_student_model")
```

## Installation
To install required dependencies, run:
```bash
pip install -r requirements.txt
```

## Running Inference
To test the model:
```bash
python inference.py --model_path models/BiLSTM_model.pth
```

---

### **Download Script**
To automatically download all models, run:

```bash
pip install gdown
bash download_models.sh
```

Create `download_models.sh` with the following content:
```bash
#!/bin/bash
echo "Downloading model files..."
gdown --folder "https://drive.google.com/drive/folders/1-nB8bQW0aQ5WoaExIzxcWo6PnhXkoLiB?usp=sharing" -O models/
echo "Download complete!"
```
