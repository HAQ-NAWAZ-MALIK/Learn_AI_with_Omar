

# Inference with the Audio Spectrogram Transformer to Classify Audio

This repository contains an example implementation for performing inference using the **Audio Spectrogram Transformer** (AST) to classify audio files. The notebook demonstrates how to process audio data, generate spectrograms, and use a pre-trained AST model for classification tasks.

## Table of Contents
1. [Introduction](#introduction)
2. [Dependencies](#dependencies)
3. [Dataset](#dataset)
4. [Model](#model)
5. [How to Use](#how-to-use)
6. [Results](#results)
7. [Acknowledgments](#acknowledgments)

## Introduction
The **Audio Spectrogram Transformer (AST)** is a deep learning model designed to classify audio files by analyzing their spectrogram representations. This repository provides an inference pipeline to use a pre-trained AST model for various audio classification tasks.

## Dependencies
Ensure you have the following dependencies installed to run the notebook:
- Python 3.8 or higher
- Jupyter Notebook
- PyTorch
- Transformers
- NumPy
- Librosa
- Matplotlib

You can install the required packages using the following command:

```bash
pip install torch transformers numpy librosa matplotlib
```

## Dataset
The model accepts input audio files, which are pre-processed into spectrogram representations before classification. Ensure that the audio files:
- Are in WAV format.
- Have a sample rate of 16 kHz.

If your audio files are in a different format or sample rate, you can preprocess them using tools like `librosa`.

## Model
This project uses the pre-trained Audio Spectrogram Transformer (AST) from the Hugging Face Transformers library. The model has been trained on large-scale audio datasets to ensure robust performance.


1. Open the notebook:
   ```bash
   jupyter notebook Inference_with_the_Audio_Spectogram_Transformer_to_classify_audio.ipynb
   ```

2. Follow the steps in the notebook to:
   - Load audio files.
   - Preprocess the audio data into spectrograms.
   - Perform inference using the AST model.

3. Modify the notebook to include your dataset or adapt it for different classification tasks.

## Results
The model outputs the predicted class label for the input audio file. Example results include predictions like "dog bark," "siren," or "speech."

## Acknowledgments
This implementation is based on the Audio Spectrogram Transformer model available in the Hugging Face Transformers library. Special thanks to the developers of the AST model and the open-source community for making tools and datasets accessible for this task.

---
