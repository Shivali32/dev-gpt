# GPT from Scratch using PyTorch

We train the GPT on a **cleaned English play dataset (~40,000 lines)**, demonstrating how Transformers learn sequence patterns to generate coherent English text.

---

## Summary

This project is a hands-on implementation of GPT using the Transformer architecture, allowing you to understand:
- How multi-head self-attention enables tokens to communicate across a sequence.
- Tokenization and data preparation for language modeling.
- Building feed-forward layers, residual connections, and layer normalization.
- Using cross-entropy loss to guide training for generative text models.
- How context length (block_size) impacts the quality of generation.
- Training optimization techniques like dropout and AdamW.
- How language models generate coherent text by predicting the next character.

---

## Features

- Implemented **decoder-only Transformer architecture**  
- Uses **multi-head self-attention** and **feed-forward blocks** with residual connections and layer normalization  
- Supports **character-level tokenization** and generation  
- Trained on **tiny Shakespeare-like dataset** (or any `.txt` English corpus)  
- Fully GPU-compatible (tested on Google Colab)  
- Prints live loss updates and sample generation during training

---

## Training Results

On Google Colab with:
- `n_embd = 264`
- `n_head = 6`
- `n_layer = 4`
- `block_size = 128`
- `batch_size = 16`

The model trains in ~10-15 minutes and reduces cross-entropy loss from ~4.25 to ~1.59, generating coherent English-style text from your dataset.

---

## Model Details
- Tokenization: Character-level
- Architecture: Decoder-only Transformer
- Loss: Cross-entropy
- Optimizer: AdamW with lr=3e-4
- Regularization: Dropout (p=0.2)
- Training loop: max_iters = 5000 with periodic loss evaluation and sample generation

---

## Example generated text after training

BELBOLAND:
That smy lord?
We will there mow we down from thy cround? Isabe?

QUEEN:
Lucond O' that the preset keep fance!
I sweet doth thought, I have shall be lost,
Thou term truch profe to givlice oftery!

MARCIUS:
No not our rushifts:
It, she hath discord of 't,
Why hear get this not thou last not the own,
Hast to in warmiated spected fame; this away;
Which made your gracious of is her,
Care is mink an eye, to Gewell!

QUEEN ELIZABETH:
If, be let to 
Paint:
And this streat then.

PETENIA:
Com


<!-- 
This repository contains a **GPT language model implementation from scratch** in PyTorch, following Andrej Karpathy's [Zero to Hero](https://www.youtube.com/@karpathy) series. -->
