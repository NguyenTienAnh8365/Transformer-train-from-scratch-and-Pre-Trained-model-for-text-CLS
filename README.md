# Transformer-train-from-scratch-and-Pre-Trained-model-for-text-CLS

## Project Overview

This repository demonstrates two complementary approaches for tackling text classification tasks using Transformer architectures:

1. **Training a Transformer from Scratch** (`Transformer.ipynb`)
   - Implements the core components of a Transformer:
     - Multi-head attention layer without positional embeddings
     - Feed-forward network
     - Training and evaluation loops
   - Showcases how to prepare data, train the model, perform inference, save and load weights.

2. **Leveraging Pre-trained Models with Hugging Face** (`Text_cls_huggingface.ipynb`)
   - Utilizes the Hugging Face `transformers` library to fine-tune pre-trained language models (e.g., BERT) on a text classification dataset.
   - Covers data preprocessing, model setup, training, and evaluation.

Together, these notebooks provide a clear comparison between building a Transformer from the ground up and using high-level libraries to accelerate development with state-of-the-art models.

---

## Repository Structure

```
├── Transformer.ipynb           # Notebook: Implement and train Transformer from scratch
├── Text_cls_huggingface.ipynb  # Notebook: Fine-tune pre-trained model via Hugging Face
├── requirements.txt            # Python dependencies
└── README.md                   # Project overview and instructions
```

---

## Installation

1. **Clone the repository**

   ```bash
   git clone https://github.com/yourusername/Transformer-train-from-scratch-and-Pre-Trained-model-for-text-CLS.git
   cd Transformer-train-from-scratch-and-Pre-Trained-model-for-text-CLS
   ```

2. **Create a virtual environment**

   ```bash
   python3 -m venv venv
   source venv/bin/activate
   ```

3. **Install dependencies**

   ```bash
   pip install -r requirements.txt
   ```

   > torch>=1.10
   > transformers>=4.30
   > datasets>=2.0
   > evaluate>=0.4
   > nltk>=3.8
   > numpy>=1.21
   > matplotlib>=3.4
   > tensorflow>=2.8
   > tensorflow-datasets>=4.6
   > ```

---

## Usage

### 1. Transformer from Scratch

- Open `Transformer.ipynb` in Jupyter or Colab.
- Sections:
  1. **Model Implementation**: Defines the attention layer and feed-forward blocks.
  2. **Training Loop**: Trains on the provided dataset.
  3. **Evaluation**: Computes accuracy and loss on validation set.
  4. **Prediction**: Uses the trained model for inference.
  5. **Save/Load Weights**: Demonstrates how to persist and reload model parameters.

### 2. Pre-trained Model Fine-tuning

- Open `Text_cls_huggingface.ipynb`.
- Sections:
  1. **Data Preparation**: Tokenization and dataset splitting.
  2. **Model Setup**: Loads a pre-trained Transformer (e.g., BERT) and attaches a classification head.
  3. **Training**: Fine-tunes on the classification task.
  4. **Evaluation**: Reports metrics (accuracy, F1-score).

---

## Key Highlights

- **Custom Transformer**: Gain insights into Transformer internals by implementing attention and feed-forward layers from the ground up.
- **Pre-trained Models**: Leverage transfer learning with Hugging Face to achieve strong performance with minimal code.
- **Modular Code**: Notebook sections are well-organized for clarity and easy adaptation to other NLP tasks.

---

## Results & Evaluation

- Accuracy and loss curves are plotted in both notebooks.
- Example test-set performance (may vary by dataset):

  | Approach              | Accuracy |
  |-----------------------|----------|
  | From-Scratch          | 78.29%    |
  | Pre-trained (BERT)    | 92.43%    |

---

## Contributing

Contributions are welcome! Feel free to open issues or submit pull requests.

---

## Contact

For questions or feedback, please contact [Nguyen Tien Anh](anhnguyentien8365@gmail.com).
