# 🧠 MiniBERT from Scratch (PyTorch)

A minimal implementation of **BERT (Bidirectional Encoder
Representations from Transformers)** built from scratch using PyTorch.

## 🚀 Features

-   Custom tokenizer (word-level)
-   Masked Language Modeling (MLM)
-   Multi-Head Self Attention
-   Transformer Encoder Blocks
-   Training + inference

## ⚙️ Architecture

``` mermaid
graph TD
    A[Input Tokens] --> B[Token Embedding]
    A --> C[Positional Embedding]
    B --> D[Add Embeddings]
    C --> D
    D --> E[Transformer Block x4]
    E --> F[MLM Head]
    F --> G[Vocab Predictions]
```

## 🔶 Transformer Block

``` mermaid
graph TD
    A[Input] --> B[Multi-Head Attention]
    B --> C[Add & Norm]
    C --> D[Feed Forward]
    D --> E[Add & Norm]
```

## 🧪 Training

Masked Language Modeling with CrossEntropyLoss.

## ⚠️ Notes

-   No attention mask
-   No segment embeddings
-   Basic tokenizer
-   Minor bug in attention (Q/K/V)

## ⭐

Star the repo if helpful!
