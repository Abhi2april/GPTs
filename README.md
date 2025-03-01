# GPT from Scratch

This repository contains an implementation of a simple GPT (Generative Pretrained Transformer) model built from scratch using PyTorch. The model learns to generate text based on a given dataset, inspired by Karpathy's `minGPT` approach.

## Table of Contents

- [Dataset](#dataset)
- [Installation](#installation)
- [Model Overview](#model-overview)
- [Training](#training)
- [Generating Text](#generating-text)
- [Results](#results)
- [Acknowledgements](#acknowledgements)

## Dataset

The model is trained on Shakespearean text. The dataset can be downloaded using the following command:

```bash
https://github.com/karpathy/char-rnn/blob/master/data/tinyshakespeare/input.txt
```

## Installation

To run the project, install the required dependencies:

```bash
pip install torch
```

## Model Overview

The core components of the model include:

- **Character Tokenization**: Maps characters to integer indices and vice versa.
- **Bigram Language Model**: Uses embeddings and a lookup table to predict the next token.
- **Self-Attention Mechanism**: Implements multi-head self-attention for contextual understanding.
- **Transformer Blocks**: Stacks attention and feedforward layers for improved learning.

## Training

The model is trained using an AdamW optimizer with the following hyperparameters:

- Batch size: `32`
- Block size: `8`
- Learning rate: `1e-3`
- Training steps: `5000`

To train the model, run:

```python
python train.py
```

##

## Results

Example generated text:

```
To spits as stold's bewear I would and say mesby all
on sworn make he anough
As cousins the solle, whose be my conforeful may lie them yet
```

## Acknowledgements

This project is inspired by [Andrej Karpathy](https://github.com/karpathy)'s work on GPT and language modeling.

