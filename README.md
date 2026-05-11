# Build a Language Model from Scratch!

## Overview

A hands-on introduction to transformers and language models. (Pre-LN transformer)

## Files

- `8_may_26.pdf` — Slide deck covering ML and transformer architecture
- `Transformers_8_May_26_fin.ipynb` — Google Colab notebook for the hands-on coding portion

## What's Covered

**Part 1: ML Intro**
- Data as vectors (text, images, sound, tabular data)
- Model as a parameterized function f_θ : X → Y
- Neural network primitives: linear operations, ReLU, MLP, softmax
- Training objective (cross-entropy / KL divergence)
- Learning algorithm: gradient descent, loss curves, overfitting

**Part 2: Transformer Architecture**
- Dataset: TinyShakespeare (Andrej Karpathy)
- Training objective: next-token prediction
- Single-head attention (Q, K, V projections → scaled dot-product → softmax → AV)
- Multi-head attention and the output projection W_O
- Positional encoding (attention is order-agnostic without it)
- Causal masking for autoregressive generation
- Layer normalization and residual connections
- Full language model: stacked transformer blocks + linear head

## References and Inspiration

- Vaswani et al. (2017), *Attention Is All You Need*
- Andrej Karpathy, *The Unreasonable Effectiveness of Recurrent Neural Networks*
- Andrej Karpathy, [char-rnn](https://github.com/karpathy/char-rnn), source of TinyShakespeare
- Andrej Karpathy, [nanoGPT](https://github.com/karpathy/nanoGPT) 
