# imagebind-multimodal-digits
## A Multimodal Embedding Analysis with ImageBind using MNIST, AudioMNIST, and Synthetic Text


<img width="1590" height="989" alt="Sem título-1" src="https://github.com/user-attachments/assets/61c705ae-3f7f-4ef6-9f72-faba2b13ac29" />


This repository contains a controlled set of experiments using ImageBind (Meta AI) to investigate how multimodal embeddings behave when representing homogeneous semantic classes — in this case, digits from 0 to 9 — across three modalities:

**Image, Text, and Audio.**

The goal is to analyze multimodal alignment, cluster formation, and semantic consistency across heterogeneous representations of the same concept.

# 📘 Project Description

This project explores how ImageBind organizes and relates multimodal embeddings generated from a small, controlled dataset composed of digits (0–9).

The experiment uses three modalities:

Images — MNIST

Audio — AudioMNIST

Text — synthetic digit descriptions

Embeddings are produced using the pretrained imagebind_huge model, normalized, and then projected into 2D space using PCA, t-SNE, and UMAP.

# 🧱 Experimental Setup

Data Preprocessing

MNIST images resized from 28×28 to 224×224

AudioMNIST clips padded with silence to match the expected duration

Text variations created synthetically for each digit (“zero”, “digit 0”, etc.)

Embedding Extraction

Model: imagebind_huge

Unified multimodal API

Embedding normalization

Dimensionality Reduction

PCA

t-SNE

UMAP

Joint multimodal projections and per-modality projections

# 🗃 Datasets
MNIST

10 samples per digit

Resized to 224×224 to match ImageBind’s visual encoder

AudioMNIST

Spoken-digit recordings

10 samples per class

Silence padding for uniform temporal length

Synthetic Text Digit Set

Examples include:

“0”, “zero”, “digit zero”, “number 0”, etc.
