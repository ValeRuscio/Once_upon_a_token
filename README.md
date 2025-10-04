# Code for "Once upon a token: how positional information shapes Transformers processing"

This repository contains the source code and data used for the analysis in the paper, *"Once upon a token: how positional information shapes Transformers processing"*.

---

## Abstract

We show that generative transformers with relative Rotary Position Embeddings (RoPE) systematically reconstruct and utilize absolute positional information, a phenomenon we quantify as "positional leakage" ($\Delta R^2$). This leakage is highly adaptive: its prevalence follows an inverse power law with sequence length as the model shifts from a high-leakage "absolute position" mode in short contexts to a low-leakage "relative" mode in long ones. This behavior is governed by two mechanisms: feed-forward networks (FFNs) acting as systematic information filters, and sharp phase transitions in attention entropy that trigger head specialization. Finally, we find that model scaling addresses this via sparse specialization: an 8B model does not eliminate this function compared to a 1B model but isolates it in 57x fewer heads. These findings show that transformers develop robust, adaptive, and increasingly sparse mechanisms for absolute positional reasoning, even when explicitly designed for relative encoding.

---

## Repository Contents

* **Analysis Code**: Contains the Python scripts and notebooks used to perform the positional encoding analysis described in the paper.
* **Data**: Includes the text files extracted from Wikipedia that were used as prompts for the language models.
