# Build a Language Model from Scratch!

## Overview

A hands-on introduction to transformers and language models. (Pre Layer Norm transformer)

## Files

- `8_may_26.pdf` — Slide deck covering ML fundamentals and transformer architecture
- `Transformers_8_May_26_fin.ipynb` — Google Colab notebook for the hands-on coding portion

## What's Covered

**Part 1: ML Primer**
- Data as vectors (text, images, sound, tabular data)
- Model as a parameterized function f_θ : X → Y
- Neural network primitives: linear operations, ReLU, MLP, softmax
- Training objective (cross-entropy / KL divergence)
- Learning algorithm: gradient descent, loss curves, overfitting

**Part 2: Transformer Architecture**
- Dataset: TinyShakespeare (Karpathy)
- Training objective: next-token prediction
- Single-head attention (Q, K, V projections → scaled dot-product → softmax → AV)
- Multi-head attention and the output projection W_O
- Positional encoding (attention is order-agnostic without it)
- Causal masking for autoregressive generation
- Layer normalization and residual connections
- Full language model: stacked transformer blocks + linear head

## Getting Started

Open the Colab notebook via the link on the title slide or directly:

```
https://tinyurl.com/257avm9d
```

The notebook is self-contained — it downloads the dataset, defines the model, trains it, and generates Shakespeare-like text.

## References

- Vaswani et al. (2017), *Attention Is All You Need*
- Karpathy, *The Unreasonable Effectiveness of Recurrent Neural Networks* 
- Karpathy, [nanoGPT](https://github.com/karpathy/nanoGPT) 
