# Fine-Tune CANINE on IMDb (Movie Review Binary Classification)

This repository contains a Jupyter Notebook that demonstrates how to fine-tune the CANINE model for binary classification on the IMDb dataset. The IMDb dataset consists of movie reviews labeled as either positive or negative, making it ideal for sentiment analysis.

## Overview

In this project, we use the CANINE model, a transformer-based model that works directly with character-level information rather than tokenized words, allowing it to handle text more effectively in some NLP tasks. The goal is to fine-tune the model to classify movie reviews into two classes: Positive and Negative.

The notebook walks through the complete process, including:

- Loading the IMDb dataset.
- Data preprocessing and cleaning.
- Preparing CANINE for fine-tuning.
- Training the model on the dataset.
- Evaluating the model's performance on the test data.

## Requirements

To run this notebook, make sure you have the following dependencies installed:

- Python 3.8+
- Jupyter Notebook
- Transformers (Hugging Face)
- PyTorch
- Datasets (Hugging Face)
- NumPy
- Pandas
- Scikit-learn

You can install the required packages using:

```bash
pip install transformers torch datasets numpy pandas scikit-learn
```

## Getting Started

1. Clone the repository:

   ```bash
   git clone <repository-url>
   cd <repository-folder>
   ```

2. Open the Jupyter Notebook:

   ```bash
   jupyter notebook Fine_tune_CANINE_on_IMDb_(movie_review_binary_classification).ipynb
   ```

3. Follow along with the notebook to load the IMDb dataset, preprocess the data, and fine-tune the CANINE model.

## Dataset

We use the IMDb movie reviews dataset, which can be easily loaded using the `datasets` library from Hugging Face:

```python
from datasets import load_dataset
dataset = load_dataset("imdb")
```

The dataset contains 50,000 movie reviews, split evenly into training and test sets, with binary labels indicating positive or negative sentiment.

## Model: CANINE

CANINE (Character-level Attention Network with Iterative Normalization and Embedding) is a model that directly operates at the character level. This makes it particularly effective for dealing with noisy text and avoids issues related to out-of-vocabulary tokens.

In this notebook, we use the `CANINE` model from the Hugging Face Transformers library and fine-tune it on the IMDb dataset.

## Training and Evaluation

The training process involves:

- Tokenizing the IMDb reviews with CANINE's tokenizer.
- Fine-tuning the model using PyTorch.
- Evaluating the model on the test set using accuracy and F1-score metrics.

The notebook includes a step-by-step guide on how to achieve this, along with visualizations of training metrics to monitor progress.

## Results

After fine-tuning, the model should be able to classify movie reviews with reasonable accuracy. Evaluation metrics such as accuracy, precision, recall, and F1-score are calculated to gauge the model's performance.

## Usage

Once fine-tuned, the model can be used for sentiment classification on movie reviews or other related tasks. To use the trained model for inference:

```python
from transformers import pipeline
classifier = pipeline("sentiment-analysis", model="<path-to-fine-tuned-model>")
result = classifier("This movie was fantastic! Great story and characters.")
print(result)
```

## Acknowledgements

- [Hugging Face Transformers](https://github.com/huggingface/transformers) for providing powerful tools for NLP.
- IMDb for the dataset.

## License

This project is licensed under the MIT License. Feel free to use it as a reference or starting point for your own projects.

## Contributions

Contributions, suggestions, and improvements are welcome! Feel free to open an issue or submit a pull request.



