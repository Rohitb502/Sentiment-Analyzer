# Sentiment Analyzer 🎭

A powerful command-line tool for **sentiment analysis**, leveraging **pre-trained transformer models** from Hugging Face and **PyTorch**.  
It provides an **end-to-end workflow** for training, evaluating, and performing real-time sentiment classification with ease.  

---

## 🚀 Features

- **Flexible Model Support**: Seamlessly switch between models like **BERT, ALBERT, and DistilBERT** with a simple command-line argument.  
- **End-to-End Workflow**: Includes scripts for data preparation, training (suggested), evaluation, and interactive analysis.  
- **Interactive Analysis**: Run `analyze.py` to instantly classify sentiment of any text.  
- **Highly Customizable**: Tune hyperparameters (learning rate, batch size, sequence length, etc.) via `arguments.py`.  
- **GPU Acceleration**: Automatically leverages GPU for faster training and inference when available.  

---

## 🏗️ System Architecture

The project follows a **modular pipeline**:

### 1. Data Processing 📥
- **`dataset.py`**: Handles dataset ingestion from `.tsv` files, tokenization, and input preparation with `[CLS]`, `[SEP]`, `[PAD]` tokens and attention masks.  

### 2. Model & Core Logic 🧠
- **`modeling.py`**: Wraps Hugging Face transformer models and adds a classification head for sentiment prediction.  
- **`analyzer.py`**: Central class for training, evaluation, and inference.  

### 3. Usage & Evaluation 📊
- **`analyze.py`**: Main entry point for **interactive sentiment analysis**.  
- **`evaluate.py`**: Loads a trained model and evaluates performance (accuracy, loss) on a validation dataset.  

---

## 🛠️ Tech Stack

- **Programming Language**: Python 3  
- **Libraries & Frameworks**:  
  - [PyTorch](https://pytorch.org/) — Deep learning backend  
  - [Hugging Face Transformers](https://huggingface.co/transformers/) — Pre-trained models & tokenizers  
  - [pandas](https://pandas.pydata.org/) — Data handling  
  - [tqdm](https://tqdm.github.io/) — Progress visualization  
  - [argparse](https://docs.python.org/3/library/argparse.html) — CLI argument parsing  

---

## 📖 Usage

### Clone the repository:
```bash
git clone https://github.com/your-username/sentiment-analyzer.git
cd sentiment-analyzer
