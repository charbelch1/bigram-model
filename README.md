# Bigram Model using Transformer Architecture (Character Level)

## Overview
This project implements a bigram language model using the Transformer architecture, operating at the character level. The model was trained on data extracted from a Shakespearean book, capturing the patterns and relationships between consecutive characters. By leveraging the Transformer model, the goal is to predict the next character in a sequence, mimicking Shakespeare's writing style.

## Data
The dataset used for training consists of a text from one of Shakespeare's works, which has been processed at the character level. Each character is treated as a token, and the bigram model aims to learn the relationship between every two consecutive characters.

## Model Architecture
The model is built using a Transformer architecture, which is known for its attention mechanism and parallel processing capabilities. Specifically, it employs the following components:
- **Embedding Layer**: Converts each character into a continuous vector representation.
- **Positional Encoding**: Adds information about the position of each character in the sequence.
- **Self-Attention Mechanism**: Helps the model focus on different parts of the input sequence, learning the dependencies between characters.
- **Feedforward Neural Network**: Processes the output from the attention layer.
- **Output Layer**: Predicts the next character in the sequence, forming a bigram (two-character prediction).

## Training
The model was trained on a dataset consisting of a Shakespearean book, with the following steps:
1. Tokenize the text into individual characters.
2. Split the text into bigrams (pairs of consecutive characters).
3. Train the Transformer model to predict the second character given the first.

## Usage
To use the trained bigram model:
1. Load the trained model weights.
2. Provide a starting character (or sequence of characters).
3. The model will predict the next character(s) based on the input.

