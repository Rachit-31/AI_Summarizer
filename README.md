# Summarizer AI

## Overview

This project implements a text summarization model using the Pegasus model from Hugging Face's Transformers library. The model is trained on a summarization dataset and evaluated using the ROUGE metric.

## Installation

To get started, you'll need to install the required libraries. You can do this using pip:

```bash
pip install transformers
pip install transformers[sentencepiece] datasets sacrebleu rouge_score py7zr -q
pip install accelerate>=0.21.0
pip install accelerate -U
pip install transformers[torch]

```
## Usage
### Set Up the Environment:

* Check if a GPU is available.
* Initialize the device (cuda for GPU or cpu).
### Load the Model and Tokenizer:

* Use the Pegasus model (google/pegasus-cnn_dailymail) from Hugging Face.
  
### Load and Prepare the Dataset:

* Load the dataset for summarization (lighteval/legal_summarization).
* Convert the examples to features suitable for training.
### Train the Model:

* Set up the training arguments.
* Use the Trainer class to train the model on the dataset.
### Evaluate the Model:

* Evaluate the model using ROUGE metrics.
* Print the summary of sample dialogues.
### Save the Model and Tokenizer:

* Save the trained model and tokenizer for future use.
## Code Overview
* Imports and Setup: Install and import necessary libraries.
* Data Loading: Load and prepare the dataset.
* Model Initialization: Initialize the Pegasus model and tokenizer.
* Training: Set up training arguments and train the model.
* Evaluation: Evaluate the model's performance using ROUGE scores.
* Saving: Save the trained model and tokenizer.
## Notes
* Ensure you have a GPU available for training as it significantly speeds up the process.
* The provided code is designed to run on Google Colab. Adjustments may be needed for other environments.

## Feel free to modify any section according to your project's requirements or additional deta
