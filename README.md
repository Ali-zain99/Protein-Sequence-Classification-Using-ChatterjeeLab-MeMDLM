# 🧬 Protein Sequence Classification using MeMDLM
This project focuses on classifying protein sequences into Kinases and Phosphatases using the pre-trained transformer model ChatterjeeLab/MeMDLM from Hugging Face.

## The notebook includes:

✅ Loading and filtering protein sequence datasets

🧪 Generating fixed-size embeddings using the MeMDLM model

🧠 Training a simple neural network classifier on these embeddings

📈 Evaluating the model's performance using training and validation loss

## 🔧 What’s inside the notebook

### Section	Description
Dataset Preparation	Loads 100 Kinase and 100 Phosphatase sequences (length < 512)
Embedding Extraction	Uses AutoTokenizer and the MeMDLM model to embed each sequence into a 768-dimensional vector
Classifier Definition	A simple PyTorch-based neural network classifier
Training Loop	Trains the classifier using BCELoss and Adam optimizer
Evaluation	Outputs training and validation losses every 10 epochs

### 🧠 Model Used
ChatterjeeLab/MeMDLM
A pre-trained language model for biomedical and protein sequence modeling.

### 📌 Output
Embeddings of size 768

Trained classifier outputs probabilities for binary class (0 = Kinase, 1 = Phosphatase)

